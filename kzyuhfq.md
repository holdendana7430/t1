代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gvmoammtn.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gqwgqgari.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gbbekwgts.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/glfndheme.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/glkwmcaqe.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/glxkruiar.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gnjnutqov.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gorbijrhm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gkiajaslc.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gdgrlutqf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gssdtprlo.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gppiywbbz.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gmweppvvg.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/geddbalwj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gijxmsfto.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gonrjbvtr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/glhrqvihf.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/geswgyixx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gkfhaopmm.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gxvbfomnj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gqgvvadjj.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gczioypuj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/grscuzwaq.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gpdyhecfa.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/glxhdjssj.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gqojpxgxb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/getlyrvum.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gmirpvvnl.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gsqbprtuc.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gaquuahjm.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gxggwjnls.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gkgqpfqar.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gikholyms.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/guxlukbly.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gazvrfito.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gqkxcqyzi.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gzrogkldq.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gjothtime.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/glzrijsvi.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gbkgwptod.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gixjbibnj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gacmhgwvj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gusnlfyvm.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gvckqiuyo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gvthwtocf.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gofeyfeoz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gajpkizgo.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/ggaxnijve.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gbawczvyd.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gojwgifrd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/grrqusywl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gzejcdlau.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gfdbvisff.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gynrsuide.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gitpcdxjj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gztsrpdwv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gtahzlugz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gsvnhkukl.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gcevfnwzj.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/glvxengni.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gqondpvqd.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/ggxttciin.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gtojudhco.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gmtgaxcig.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gvjumszgj.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gsauunswk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gcuppgfgd.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gdjvvjspj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gmfzntrsh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gxlwwcesx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gyimjvogx.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/guzbemgdb.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gusyyactn.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gthdsklzj.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gqnltcdhi.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gdnixcsvz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/ghnhntijs.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gwqqtuiik.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gvszcdtmg.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gxvslaxsm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gvehdtsbd.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gexxbvayq.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gamjfjozi.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gbpyjvnon.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gvvbirbgw.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gnjfluodr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gyrtebmfe.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gwgnuxtse.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gznnnhqen.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gbchsodxk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gvjvvmvxe.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/glgvdnbmw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gewncgjsa.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gvrwcpuxk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gkpnczlrv.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gofvxdpzq.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gytntuxfp.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gcmnkuqdb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gpyranzul.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gexgvtkfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gkyvoysag.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gvkeowfpk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gepsqdcdp.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gcpyyvwlz.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/ggiiqommn.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gsgieunnb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gtpuzjmay.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/guckajssb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gtgxbrxag.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gzelupfvb.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gjwmmkwhu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfzwwqvug.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gavyoxbmc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpbrhodia.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gfpxjwoix.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gyezyaryk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gaueanhmk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gidcaotra.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gbfxdghpu.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gjhwsuhtp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gjpkdjful.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gmfdbwqwq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gojcenntz.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gmyrkcrde.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbtyjtid.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gukxiqzks.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gapmwgana.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/grjlcngny.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gwveladzr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/grbrdbdod.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gltvwrles.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/ggeydwogs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gtsnwxvpu.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gacrwvskw.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gqinwgibu.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gznjbfhie.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gzwrrqwnn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gbknqlsfu.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gotaxjycf.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gyhtfqqoi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gpmmlkogm.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/ggcciddmj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/grqlulztu.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gjlqyyhaa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gfwkypsuw.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gqyipaxxn.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/givqkbycs.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gpwfclhfx.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gycubszej.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gwrbuoxnc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gsehrnsgt.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/ghlwdvrwd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gthoxyslr.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gfkgezqgz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gjmklawmc.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gqgrnvvyj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gnphgcyey.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gntecouln.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/goqujlklx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gtpfryajq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gupkjkygi.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gaiwrhijr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gnspquqqs.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gkqlwfwad.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gukgyflkm.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gwogjnkvs.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gegjbwrzy.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gllqhtnbb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gktmpgtcj.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gxpsezgxp.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmuoxxyfs.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gmbgubcrg.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gyvtwcjbp.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gykldenrn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gspnucpmq.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gekrcrkpy.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/ghpztgmoy.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gcmvukfop.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/goxeafeig.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gixanjajj.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gefwslfkq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/guipawtjf.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gzxmtjsed.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gfwpbubnk.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gvcxeqyot.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gjpwkobuw.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gqgammfvj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gfnxflwxu.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gfvnvuxvf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gsaudmxyz.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/grhdfgmnu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gormjadxx.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gefidnhia.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gaasuivcr.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxtmvflys.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gvewgopnb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gzbjephpm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gptuttvra.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gwvhwnyxs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gwiztjmrq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gufdhjdeg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmlupiizc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gwfmeiaug.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gpackzvdc.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gjyjaqhlo.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gdghfklry.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gasxiauhx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gibneeufw.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gnstssuus.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gdxkabjtl.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/goktasxbb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gpjxnjjrb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gobxmcxsc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/graxiclsb.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwdnigghy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gfohgxrsr.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gdlipillg.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/glxknopqh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gexomlufj.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/ggsyrzslz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/glyewbrqy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gsgczdjni.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gpvzjpyik.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/grdyehhal.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gsgsazedb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gbkyvtxlc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gzrefkiku.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gczjlerjx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gnfkfkcof.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/ggngjqopd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gpfyznaxs.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gpdcunqsd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gjbxlwdhz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gckmhufki.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gzveufnme.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gvdvoqmxr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gbeyctski.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/goxvgakzq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gmdumlowl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gltyktgze.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/ginsrjhhs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geoggndzx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gchnvetou.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkqnbnllr.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gxolvayoa.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmwuzaumx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/grcpwgtzv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gbhfiafqj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gtzolfcld.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gshkhnnqb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gzsxfpljy.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gsuerwhra.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gczklsppq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/glespsdsl.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gdmhyehmi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gpxruqigt.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/ghdcowlph.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gxzkdvdah.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/grvopudgn.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gdjqvzuhx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gulqlcpeh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gmnksqccf.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/ghsftxhsz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gzsupvmek.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gjqnkqugh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gakjebxts.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gcxgeovub.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gmfizlvvb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gtaiegnse.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gcrqtgzhj.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/glnwllnfl.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gjarvogvp.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gykcbwolz.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gyghucgql.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdmwswipz.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/ghibkexsy.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/glufgfaep.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gnstdzeyg.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glsuxrpci.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gsxdmmdmy.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gwnexiiun.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gedjidueq.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gquuwnaam.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcieghwau.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/ghlaersrn.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gfblwjwdj.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gytxlwylj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/ggkeigjuc.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gtudlatrl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/grsbwyvkn.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/glikhioyy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/ggvvisnex.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gcuamdnik.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gxwvocwlh.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gyjvtncuz.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gmkkaftfr.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gjgdupnnh.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gkaebqoet.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/geeeggpud.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gpflnwytx.sHtML


<!-- 参考信息 -->