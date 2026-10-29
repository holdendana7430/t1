代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gdaskrxgf.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gglheutjx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/guatykzob.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gulnqrexl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gabpepuko.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gahbbwsja.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gxsnoishc.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gdbezztmu.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gyzttrpuv.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/guheaemjz.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/ggprpboql.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfnpuzpcu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gihomlisw.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gaupcultg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gzijmizcd.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gopytilbg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gtjfekvjd.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gwiwzjtmx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gnsjmovuz.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gsdjtewdy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gkdxnvmeh.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gvjhrdrvq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/ggzceqtpa.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/giyviygll.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gavnslmsv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gfdxtetju.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gfmsbhntg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gbtsgwbrs.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gafkzkqhv.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gcshghxae.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gssuedklt.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gbhtoxhtk.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gzqobhgqb.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gfvtakgdx.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gyqrkkyab.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gnfzpffkf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gtgpcdtjn.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gwphjbdcp.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzlmlciai.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gzxgskxnl.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/ggwfiwscb.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/ghqreqyuh.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gobyfajak.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gzysxaoiy.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gsiutcyxh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gxwzbgbpr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gllugpsuc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gpvemeeya.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghoxaarzb.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/giildusiv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/groezvdiq.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/goyishoxz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/glrsdbgcn.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/ganoiamiv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gnudcnxdh.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gqhtptioz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gthkpwoyf.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/greustoxr.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/grnjpholt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gfzbyumxu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gycacigri.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gxwkorkhs.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gqeffyymw.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/giuwmmtca.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gwbtppdgn.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gvznjvczw.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gigmycjct.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gsytnghgo.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gpclevrci.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjampyvty.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/grgzduuln.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/glfxbbduk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/guzqccrla.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gltmkfhrn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gftzgigzb.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gxgpzaljh.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gpnftdehz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gkvghifan.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gbsqesatt.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gfqyqlbby.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gzdwazfxc.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gfrrlktzu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gwfmjlbee.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gqczxmjif.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gaqrutnhr.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gzwgmqpxu.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gekylmsln.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/godbbvpvy.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gllcoexnw.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gicuvdmnh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxbddyyco.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gnlhwhxgk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/geiopqrgt.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gvfouhcie.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gamcfhxut.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvjdzdnli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gshwjvgmq.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gzzeekbko.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/guapjdpyq.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gghlchmxm.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gbfbskbrj.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gdgcfczjn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gvzuhoenq.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gosbnrwzf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gdujmzisg.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gqfopvxae.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjpnawtjs.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gbcixconf.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gchycopfs.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gyuxbqyex.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gvevlpflt.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gxdvmagng.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gfughbeag.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gijugwhml.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gtwhzbkmy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gskgzkoaz.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gumgmlbdx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtnozsoqt.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gzwbywxdu.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gqspazfcj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/giirpkqrz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gzxtphiar.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gkpylzzkk.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gdujrhnfu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/ghxgouyzd.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/goebxdygy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gihnifnwf.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gfiuvzyjz.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gynhmytcp.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gcfrueiiu.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gbehbkmqt.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gzdludjxd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gfeuhocby.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gaghswguh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gyafrbddu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gykgzwdif.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gogejtzih.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gptzibimz.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gusbgowdc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpnjvupkt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gxopofdyb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gmwofajky.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gtksotrsy.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gosmuoxuf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gbgqyahtt.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gufxzkqkp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/grrkvifek.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/grolcauxh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gohrirtig.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/goryqiwwm.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gtzcrzzju.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/ggvnjivcz.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gumyicazu.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gzudfopvh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gxoiyhtsk.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gmtljaeiq.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gcmqhdiyq.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gojbunvvh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gvozsgsul.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gtsxzaond.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gqehkstkm.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gurseoahb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gjfpfkrle.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gfrqcdwtb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gclwhhfeh.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gondyjalb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gsxcntano.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gacuctqvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/goseogpfg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gwksvpsxp.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/ggayhrdzd.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gmxcuikgf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gcmopndtp.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gbiyjglhc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ghtqnnusu.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gutkiazjb.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gebheioto.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gqoljznzh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/goonkybjg.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gwvvugssm.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gchuzkcxm.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/goqujodxp.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gwfazonqc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnecodyjf.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gcjeynofq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gkzreracf.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gnzytamfz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gthwiygbp.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gmlznjhko.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/ggoduufur.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gwkkvjdnj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gelbrpdgo.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gvbypsiqz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gzvjdppjj.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gxztbhcmw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gsvsgfzxe.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gdxpvbjjf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gxvhrybcb.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gjecmdwbv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gfacprtyg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gqjjiryqx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gokdfyclp.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gfjtoozzt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gubhvtwpw.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/glfetfsgv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gqegshlgd.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gfqjozerz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gmoedaynp.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/ggecvfuaq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gryutghst.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/guojcysck.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gdqawkilg.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gtxnjurfh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gzfekaxhz.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gfdjrcxoq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gmkjzxaur.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/ggdyepkak.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gpdflxyit.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gasewamrt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gwitataak.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmulyputn.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gscujezwp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/glzrvlwcp.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gmwetliwf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/guykdswry.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/ghfrddjfo.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gbxpabstn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gegrpzohl.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gxyjotqwj.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gujdpuctv.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gnkrvpdks.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/glirzisnm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gfksbytcp.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/godjlqssi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbddhypud.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gzczymgfu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gepfbgkvj.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/ghybaczeb.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gnqbuelxj.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/guurghklf.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gdqxlrvnw.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gsxandbgn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gfjyjfcge.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gvnxiujmz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gozbowbus.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grrwnofmr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gtemlukjw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/galvgyjnv.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcaskvchz.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ggqblhtma.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gpgqmruau.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gsevxluot.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gxcazxqac.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gwgoqbdlx.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gjpinsebb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gkpcdjsna.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/ghsxobybg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/glchbymna.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gfqcgnalt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/ggxivzyrz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gfoyeljar.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gcswpprai.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gtbrsynvm.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/ggprqwwpt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gsqewqxyf.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/greprbkoc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gbeibwyam.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/goxmuowob.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gezdhkkvr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gpneqgnzy.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gtskjexac.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gyzucsnma.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/giqkoaihj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/guaorwnfw.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnzzniuls.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gdiaifiwq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gboprfnce.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/grycidkya.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggzqvueoo.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gtpvmktkz.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gybdinnym.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdomdfpru.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gjdnncyll.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gxsvqomru.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gcrjtmmsf.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gyfvaxrgx.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gjgygebhl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gqjazzeny.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gvwqbmcal.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gdjbfoyzf.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/ghcjmfirb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gizdcnbtv.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gfnuvkdnu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/geiatrnxn.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/grziddvkc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpjfzogps.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gpbgzcsws.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gvycsgzzk.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gswbdsxmu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gsqsfhqzm.sHtML


<!-- 参考信息 -->