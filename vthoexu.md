代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gucihicgg.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuzhcuhq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/glvcokypm.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gifluhitp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtotstfoi.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzqxvazd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gehooyqrw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gnivhtvcl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gkjkspomw.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gupkueejh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzzjzpwcu.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/guhiabmqf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/grdbifzfj.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gygpsdtxg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gdzwtgxeg.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvlszmqdi.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuoixlbh.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjcfcgxdw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqvcnarm.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gmbljzgxx.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdufafyxr.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gfusccupp.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/ggpuifzve.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzvluhii.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqekpxtju.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gmziwbivr.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gihokbcdb.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glrykhfsa.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnuattmc.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/grzcranzt.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/goxpwaqtu.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gsmzhfyzd.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gcswxntrg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrwibscr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjhjszei.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtyhxvuig.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjnglywe.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gykqrrvkx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcvpvjvp.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gendwkpmz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyznzuqb.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrbfpkpd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewvxwtjm.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnuirepq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gjejmwpnk.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcmldfhp.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gucllxhfb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gunnyldaq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhruldhr.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrppouva.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuigidul.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ggwjutpou.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/grkkzzcxz.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gxrndghqf.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoffhnhi.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gatnwcspl.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gmystlots.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlglxxxy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gxtclnyjl.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/grzwbylpv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gxdhzlyfr.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsoiqkpy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/grelqnbay.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwvtknxj.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/glbbtdtof.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gttrpdyie.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gahwhosdu.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxpjzyik.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/ghyiqekvp.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmjismtg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gluttzwwm.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gnssujauq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gwlvlhfka.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoyspdrs.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/geamuyedk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmgmvehq.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdbutdhu.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gozrdomdd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxdsepla.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gdnikwazn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkinbzox.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gognkdbtg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpwmhtdj.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxcwyaji.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjdvavbd.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmaazvcg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnhykrer.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbtpjyhi.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gsrgizhxg.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/giedraoyy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneoiifvc.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbwebgbc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gaezvbvvi.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggdhhjprq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gicudvhsm.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gaugibarw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfceipqux.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gbmlzbqrc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggydhcnlm.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/grjdcrlms.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grczgumhy.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gupwbssho.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwtmtkrl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxnsblme.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gekznktlp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwiiqelrj.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggjofcqsw.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxhbowds.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpvvawlc.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxoxhxih.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gfgphvcqh.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuidshso.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfwlwrfg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrlutojt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/ghczhhzzb.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxujfmaay.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpwrsnvq.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/grbqslzra.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpgcryyz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gjszergxj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjvkwynm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gdqzujztc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gxbtegoeh.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/glevjsiuq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gavphuoia.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/grfuqrywt.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyhdltkd.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvrhcjznv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvlugmgz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/guhdyklsp.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gfasluwui.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwhkvikuw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggupjadah.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/ghfkkswuw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gezpbvvli.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gnziajeug.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwipoxwx.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gepwiwypk.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayqfffly.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfenuikn.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gksmhbgug.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goktenqcp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gdlqkdkha.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgivpnpj.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gwdryvqre.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtmmmngpj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzfmvvuj.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gqjsqorzh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gugsuaice.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gddouxluy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gjsarcgft.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtrlnygq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuadbqfb.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtlrxflc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfwzvimr.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gipdxnuot.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrgczuoe.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gpbwyypum.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/glcwilium.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeofrrpu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gemqolarm.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbrgbkrt.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyviephra.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggajxpnhd.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvgjzwxy.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyhtgbwg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gocyqztls.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gltbyshcv.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ghrefdpss.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxfumxsv.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmgrwana.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueroqohe.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdhelogz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtdotedoe.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gpsycsska.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyafxqip.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlknpili.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ghbqkdfsi.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/guyowvpar.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggludhtvs.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goggnirex.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmztjmvh.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gyzkkefsb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxkwnsvt.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixbaejre.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtwkvpac.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/garolrtzv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gwbudbzbh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gnijftnek.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gtuqigncc.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gdmlpaiqk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjsevqlz.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdgwqjyi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuxkqbow.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gamdidimz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gwjmubvdl.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuhiipti.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjunsiyd.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyevwqyhf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/goqutqpyo.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/guqyhbbsy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gfjlasqgb.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gfvvdvasr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghpibjeyb.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gjsnpaatg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/goprcviwx.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzklbhipb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/giedqyxpu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gxgkpqiue.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpwhgarlm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gzxgohpfx.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gqowlkkch.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdcmctdi.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giciwfyll.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gijykfogy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqxbwgiu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gijrsotta.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gtplckogq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/glqbhhvkg.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gatujqnar.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjycmkarm.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gczfjuziq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gawjlqrel.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gejnafqwe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvfpbgen.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhhjrbmp.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmcaqnhm.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogdbzatb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/ganifilio.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrhnnork.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyjmcner.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gahbyeyjm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gkypimniy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdkfzlyzi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksmovqnq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyrxgbdut.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbzmxddl.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/glwqzjnna.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwzycghh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsnvrhdg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheskrlcu.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gxsxjervz.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gtvxucznl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gewiaaryd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/goadwnqul.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbggbeqx.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnmduxtl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjryphkb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gurxphxos.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaomxujvt.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gztowqjbn.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gciuuafrl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxulomgrs.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gwqvxzegy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gycaxstlh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/glxinyzvi.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gyxovquxb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/ggabknobp.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gcllhurmt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljoiftgt.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrrlwkry.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gloxcohvg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimaruvyw.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gwucuaqyw.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhscwjej.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gizufjqyg.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwexhjhcq.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcuubuel.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gmlmfkpal.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gikqoqrgx.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjnosvmh.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gmdcnkxbl.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gjvjrxrul.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gnvfmmcei.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gexkxgsck.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gkiaersqp.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/glwzybioo.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gkkfgmblu.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgelganq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gitvnzupk.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyocktux.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gkayhywby.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gkpyxwafq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqkhkjcc.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfbuqixs.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtponiphr.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gbjjpurcy.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpwcqjzx.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/goinxvylq.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/giqvesjys.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/grxavvyzd.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gisjrfhan.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/greisvnsk.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gxcsskclh.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoloozcs.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gebqbktit.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgtogrwa.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbjqlvivi.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzypntnpf.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gymbwzjsy.sHtML


<!-- 参考信息 -->