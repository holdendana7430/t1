代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gdwikidud.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gkowegjjj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gvlzoxppi.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/glqeqajbl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/glijeyhno.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gogqwcgea.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gwogeehrn.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gvqvmptae.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/glvmznymm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gosdrixvm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/ghnvkskuu.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/girhcxdbs.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/ghyjwtait.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gugrktaoz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gqivnyqrt.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gfmakkrvm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gvbladert.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/granfatoi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/ghpfjgrgk.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/ghwmpvlfo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/ggjdqsyuk.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/geybydbno.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gtnjefuwd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gpyndieni.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gpptjmemf.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gwbwnlaga.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/ghujtlfiv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gyxwllmwv.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gyvduyxnt.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gdixnghll.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gxkjsxsfn.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/ghophrqno.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/guvkhfapx.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gaxavkicf.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxpbojide.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gbwutkokt.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gzdpdcgtx.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gcqhruiyb.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gzxdrmgcv.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gvejqomkd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gixhqqomu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/ghadqyppd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gagjdsbzr.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/glwzzsuea.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghicdvkku.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gnhdmrmno.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gsldsfnab.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzinepksv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gorkfgcfl.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gtrsciozr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gqbiwcodm.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gqbmkwpax.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gaastcely.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/glekdlbyp.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gzuxbvllc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gopadevxt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gmwsagdgr.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gllmoutgy.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjqpczcku.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gwfacrmca.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gcwaiuqgn.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gqextkrml.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gpdgwziva.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/guorypktl.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gytkxzsjs.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/glnjsjfkj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gclghafst.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gfloytjai.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gxlpiugmh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gizwzljui.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/giwxlntuc.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gacbcxuyp.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gsnfvfowo.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gycwjtacd.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/giikwajmw.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gyeyjmkpz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gsoumspuu.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/grggjlvjg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gnrzbuilk.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gfxlggjmv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gxzrtwniv.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gvvgmknpt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gfmwkyesg.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gajrgqkbw.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gmwrrcrko.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gqldlavgk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkjejbbnu.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gohtptroa.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gudtczczw.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/ghxqacwkm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gnsffhmog.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gtxaoywvt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/ggtjdfjhq.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gfqbzydhh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gvgxyveqh.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gjouvodmc.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/grwhreqnh.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gliumcroy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/glrwszcxw.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gmzuraahq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/geidbxzzj.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gowalezmq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/glfxoobwt.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gnwamorzp.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gkyxveobk.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gxdhwpwyx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gyjonlgna.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gubirojrb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gywanaltz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/glttvhhsm.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/grstxdonn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsxnmnjbl.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gwslapmxi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqxiyclkh.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxavdcgsw.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gbdzdckih.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gapfqjbsm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gynauetqi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gaxxfhorm.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/grdnmkthx.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/grijwvbit.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/grmnxpcwi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gsjglkunn.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gwfgnovys.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzsfgptnm.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/glojswrwl.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gzpufmndy.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/ghrydsecg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gfzzerekw.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gipqdmlwr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gqfefufjd.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gejiwsibr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/guopouppi.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gulognafx.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gpztulsly.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gslwydnkm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/ghbktdspv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gxtasarvs.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gjcierech.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gwseyxwpr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gjpbppuoj.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gnyjkguyy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gjzuetimj.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gmuvxzqhw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gflobwdhm.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gtssknayc.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gqifwcbfp.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gmaylrqft.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gvagxkmri.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gszzkanrl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/ggkpxqtbr.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gclyofljm.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gzewpadoe.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/grsyhyiql.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gohcgpxhs.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gcxkdslbt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gkatwwyds.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gbtqljlva.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gfhrkyqps.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gghmiyvie.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gvitofdts.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ghjmmcrnn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gchmvgfsc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gxiqxatxa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gywyhvewg.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gmgemurgm.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gegwpdbrd.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gbvtkzmmr.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/ghhorvnhz.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gjbatqdoh.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gkekmmxuh.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gnpufmboi.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gjcjbnjce.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gzziblaic.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gglrkblsk.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gdysovxtx.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gxvlfwoim.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gzefbakmv.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gtdyeifym.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gaqxvzlyx.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gwwfhpfzs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gicbqkmvb.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gyifygwrb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gxyfqwcyo.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gviozysru.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gpxqlrbrb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gawjqjyaq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gqyaehiwa.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gdkgalxks.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gueljwxva.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gklsdehcp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/glxitxtuh.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/ghpzrafyx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/glxflsuey.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gugnoiewe.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gmrtydatr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gnybdddll.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/grapgrimt.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gzwsscama.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gbfqcusmg.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gyycajept.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gewyvihgb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gojcjprqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gsgveholm.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gmnhagkkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gtombdlun.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gunkrhrkm.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gjtmhqqpk.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gzkvxvlgk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gegtfmzmt.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gmqdjcpsj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/geripbwom.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gdcqobddn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gvemkzqyl.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjcflqzpg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/geifhwgzf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gkansfvfj.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gsidinwax.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gvvyxlquf.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gnrdbgbrp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gmbvwjmdy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gezjuybmo.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gkxhivevg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gxzstkeyc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gborkhnbs.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gnypjonsm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gsjvbrqfi.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gmigruwkj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gmabjrmrq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gfkgskrvn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gmyefynic.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/guidzdtxd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gsjmmptbi.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gjavrhwsg.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/guxjnommx.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/ghljwpzrj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gygjkzfew.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gytfbqqnp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gclnohzhk.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/grdppqyeu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gmufceupi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnltihsjj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gntbprnjh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqafqglvo.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmrmbahdu.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gqpngenwv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gcbjyvvgd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gohgpkvko.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gimrzddrm.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/giixftois.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gbdfxegbw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gveivzmsv.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gwzfkpgen.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gmaeqntgr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gjkfxkxwl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gsdefkebb.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gjtxjxwjf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gfjhltymc.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gbrtrgxzd.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gkraxrtbf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gjqwvflmv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/ghmiwgems.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gnbxzwzax.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gsfigkxac.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gelnuxuoq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gzsvgacij.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/geadeettt.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gswedcnoc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gqfdouqgq.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gofedsmag.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/ggunwfdxc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gudoucrfh.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/grqdzcvuo.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gnkqqivhu.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpxlltmnz.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gmoaoevlt.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gqymnwiuu.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/ghkhmcanh.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gpdsrdjon.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gjpldeeip.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gqxmcscrx.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gjutksvik.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gmajyjblc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gyytpybvs.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gpxtebexf.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gwxnefvql.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gzdgimhlv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gvgufqqhs.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gwpuqndau.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gnzcdzyaf.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/grgbporhm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gbjriimyy.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gqbrezwvh.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gxegeodwe.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/ghmtyyxfd.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gabbhltcv.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gkvtkhqno.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gunsrkcfy.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/grgdbygvw.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gtfmgnfaf.sHtML


<!-- 参考信息 -->