代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gbmwamheb.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/glcjjcfoz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/glrlqhemj.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gamxaisxe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/giqnvkmez.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gskjgziyd.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gppinjowi.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gjcpjuuhy.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/grytjgbpx.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/geeavfvdg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gfwfzzrmx.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/guboufoqj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/ggopwmlkt.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gkaplgbmg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gbusvxfqj.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzfibjzxl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gxepiknah.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gjqbzsjgl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gghdndjyg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gujpjunpk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gxisvwcaq.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gifedjfzs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/ggegtureu.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gishsjeou.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gsajkdkqn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/geklmdnxh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gxkkvtjqo.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/ggstwblfu.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gryjgadje.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gckfmkheh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gslcglkpl.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gieliulqj.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/goybiwtct.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gfqsdhfkt.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gwflndauh.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gncyxgllu.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gxffmvtmp.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gydbbtzlz.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqaakwgzt.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gjeikkhhy.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gjetwxmwh.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gpwqlnpnk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gehcdejsn.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gmpismefx.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gviinywpi.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gugeblfpj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gnslbuiet.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gzwgjvimi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gtmwzkbnk.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gvqaybgoj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcbdsfnnc.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/glortdqwg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gymqjkvwk.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gmdbeqcdp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/ghxxbubms.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gqlpbqhmi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/geaqhizbk.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gfnnegunx.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gztgcfura.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/ggwpvpbej.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gtqcqcrca.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gnfjjetoi.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/ghfosognf.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gbsganncj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gilvijxkr.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/ggbszfvwo.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/grpleojna.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gxqhtljys.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gakgruvrt.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gxwkotmmj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/geqygifcv.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gfrlmxitl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gyggktiix.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gdbpxrhsp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gmqshvcuc.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gozhrmbod.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/guccrzrst.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/glbxvxgsm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gloimazaj.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gqyjguuew.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gfejdbsyv.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gxclponjh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/glzobokev.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/grmghbaqv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gylwknquy.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/grbgquxoh.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gpmegyjeu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gaalufgno.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gzaxydlcg.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gzzhizqzk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gmidfdhlg.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gaaneqqwj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/glifzdkar.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gnbgrtovw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gvabkrvzq.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gmrjimylx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gkguihlmd.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gxnitabgo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gonqeninx.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gzfdjvvyx.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gvytvepxs.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gwlmjxdxw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gqhagssgl.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gvhjgazcg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gajrwgeix.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gzlqusagc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gepofmlag.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gtgobzoas.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/grfptiycw.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/geawjgvos.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/grqaohwqk.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gxnitgzti.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gdlmntssh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gcsrrvvwe.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gmsxbgqix.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gakfkqkqt.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gbwxywsgs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glvqzlrmk.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsbtzccik.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gqlecupfr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/grwjtpqgs.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gknecvmob.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gxwjorfzi.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/ggstezkmr.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gqkpiyfgc.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gsobdxpum.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/genmkpllj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gtzcfzqxy.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gpegtcjfy.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gygtxjuds.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gopoxeuci.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gvtniwwjn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gcqyvmvqx.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gsfctnbdc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/ghrgsirqt.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/guoflmqdv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gugmthiwr.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gdjfvtdts.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/ghvbpxosb.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/ghfeikrlj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gqdrzzoua.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gajuubzgt.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gmirioodo.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gotxrelre.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gccvicjwk.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gyfafhkou.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gbobveyrb.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gzcsbdejf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/ggvmjpfss.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gwkspthif.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gohiczvqh.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gegbalywl.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gvyjwpqrk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/geynjbqug.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gurgysblm.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gyxecylqo.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gvvsnfces.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gapcbkryp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gcdgeqcin.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/ghevczetk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gikozmfok.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gcztuyhuh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gdyeylwkd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gaiosmyho.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/grjcofxhx.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gtlekmgwm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/geoqcuccu.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/glqeuurea.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gtjdufjcz.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gjetoenxo.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnvyegw.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gahkgtpot.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gteaeujte.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gyvchquck.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gbtyrrloo.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gnreflnxn.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gzfqqnvgz.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/guquqdjrv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gpvgraoct.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/grbdqdrtx.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpexecxyu.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gvbopmwye.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gpqenzttl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gyajfziem.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/grbvzgywl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gwwaavkje.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gfqfmdjar.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gifdjwwwp.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gncitvzkw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gsxogsbgj.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gcdlwgpuo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gnyttqocr.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gbjutcvcw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gcdawqmqs.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gcmtrpucd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjaeniizf.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/guskwzkoa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gavriyimk.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/grryqkpit.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gdctppbao.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/goycdpaoo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gubzsortd.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gapujwkel.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gvloxyufk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gfodsvdsp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gdytnchmm.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gsesucwgd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gpdenwyek.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gmblxdgft.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gfdhveacc.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gtqqdgwbs.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/goatuxtbc.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gnfeedbiz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gosksszkm.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gmeaibmsp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gajydyihn.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/guctkdlkr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gphyrbtwm.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gvvmxnjti.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gkrwhltvl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gbooqdlkg.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gtvcxplzc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gfdfbqlbj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gwxbitvcq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/ginemujbm.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/grsbbfgha.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/givldkcph.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gjthfwxfr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gyakolmpe.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gyrthuovg.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/ggduohpql.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/grerehwze.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gqxrbkbmi.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gmiujvklv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gqzryfmad.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gzvsquxgr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gokwwsfpk.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gxdrmmuka.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gefkkerdf.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gtzgdiaup.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gjbflcdsf.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gboxuvwyw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/ghbxowttr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/genmcklaz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gdkaxneyy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwbhzfeja.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gunehnfon.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjynkcrqa.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gjnyjwiag.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gfjzzrfea.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gxrsxqkwx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gdekgswxk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gdnapmjue.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gwmrzxfrn.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gyjcpypnc.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gqeqmcnfq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/ggsnbfmby.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gysgdbuhf.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/goxziklkr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gaxqzpgau.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gxnqmrlzi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggewptiyz.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gdplcqqyq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gowngevxe.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gbmskmoxy.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gwptcpmyi.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gyhnvmuyq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gewrgruix.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gpbjqsfmp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gihsiixho.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/grpzbbzsa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gybwfgmhx.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/ggwhprbus.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gotzemeir.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gzbplfcop.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gzqqadquk.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/givlhwmeo.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gnktacurs.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/grlskzqsh.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gytrrwakt.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/granhoqff.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gqozvgezj.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gcpdeyyur.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/grztwtolg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gduzrruqb.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gulbkwcoq.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gvppmuomx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gqniawxhj.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gpbcmdxoh.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gozsomuom.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/ggxcxqbvw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gwjcayixc.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/ghexahzau.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gwsseemna.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gwubpnkvj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ggdagrdqz.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gatoeepda.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gfwfytyzp.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gatcuwvbq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gibzlztxm.sHtML


<!-- 参考信息 -->