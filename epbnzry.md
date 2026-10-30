代发 wailian999

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqxsvebk.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gaswxfhyq.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmjezccop.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsclutwtz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugswfkwm.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgxkauyf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwjhkiwv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/glfuizcub.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gusidlxdi.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghyvpwmkr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gdsxpoltf.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/goknjpuia.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gepnbqebu.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gzjxjienz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/glmfutyvy.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjpqboryd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmycluwax.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gljadvxyl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcldtabzj.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtdncehr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszjjqvsh.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyvqrvuj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geyqtqmxd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gsspwcsds.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmdjhvcr.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gpwyddxsp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gthmpyxpq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzpwbbvz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcfjdjxp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpagotfq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqbfztls.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gauxoglnv.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtjajheva.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuxwpcnn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gldxbiovq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxivhpzr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzotnmnzv.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gozohzshq.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/grcblcmbp.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlejdcpe.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/guydzveqc.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlqwmpsg.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnqcoujo.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzxzwxxk.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gqkdzqzwt.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gohfrtcvk.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gfkfkgrbj.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxcixshu.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlznlrva.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gwusatdzf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gqjoipgpn.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gozqitrdq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsugpwsec.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfygpzxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwucmlgje.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyozvqsl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gxieizbes.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/giekbeojz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyujvjlm.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurctkgee.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/grhjcfgxy.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttoziufn.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmqvlegy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gfmvqpceg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gipkggcjb.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gexwvdjhi.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwubpmci.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggswikrlf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwbgwdkx.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/glmqycbxp.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gzqqcrraz.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gvneswbkf.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gmnsgbcml.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjnnxlzv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhxhcpir.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gonwfnnuv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gtydsdvbh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gagzswoic.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gyjeurtnj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfvkwjnf.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gssqsjslh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrtflevq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgzqbchn.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/grpzdpndw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gzdswbzaz.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqujdlhl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gwbimraob.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/giftyuzof.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gzihriihd.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garfxheku.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjacpnuxl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/getcahmvx.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gjvfajvsy.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/ghyiaratp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsjpcpoe.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzprjedv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqkfgxpd.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/guhzyheyk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeiaoatq.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzxlxwn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gniienzta.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gnqsmzxjl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtiackrae.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gyyyrzagw.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gkohifzim.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gorlurjye.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/guavtlkvi.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpndauquz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gggtafrlx.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdbkigrad.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkjslyqy.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvxbarni.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdfgmydx.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gruowlojw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghmdnxkwe.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gfclygoxq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gytqdfrut.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfkxtlrn.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpxtocdk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypchsbso.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gofeedykc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfkvmapfd.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guoldexpn.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gexvgulkc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxoyugfu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/guflujpnz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwltxxdya.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gqpainpfi.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gypixseqm.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoldksqz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gqvvuohet.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcyrplous.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcrysmowc.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gybsizpqo.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gqxnbnomk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaogancx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsybosny.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvyvdfto.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gukoriecr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjatexhp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/ggerfurmo.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwledurxn.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxejhzzy.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbquuimfr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gcohubnwp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/girmqlbhw.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfrwljpc.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwejwjfkf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gprjpotkt.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzcexmlf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwtmlvdf.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbwtkyis.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuuujrqw.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtbleund.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqgyinpt.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gkbjubsll.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkmyiyhg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekzprbgg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gaqosiuam.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gobuszfsz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsxgyzgt.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnrfdsuhm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/guenwbjmy.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdgdpkxb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqegtqjr.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcvnavlv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzrsuktl.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhuorufm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjsdbtop.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnofshrp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlxltlku.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaxqsmgp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/grpqxrwet.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gaxcoywtw.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gushigmrf.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjipglzd.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gegeatzzc.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gksxpeijy.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gyoidizkj.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnqaiqvyz.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsggutway.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjhkquqmo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuedptka.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gtehenrwo.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gocuaazee.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/guzqgkbng.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyspmchr.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkqpeaoo.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/guwbytsai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnidkrnor.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhudqlfh.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gyddoyktb.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gxgmrrwxk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnvhhqpdb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giouzhrqo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwwxrhgeq.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhclcoxk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwewqdti.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgdfaldw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncxjajgy.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxgwqqap.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ghvrebxle.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmiszids.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghorshnnu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grrrefsue.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/grmotqicb.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqkeride.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfsymuhs.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqlpiwtz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gzedjtvzp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guysmklmx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrodrabl.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gfbgcckaq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhloxhcb.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gjocwphtq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzshetxtp.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gqytayypw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggieizjxw.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gcchguvvg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtcblouu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvzsigyv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayrhypzh.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glkkqpejg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/grelyjopv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gaefzaevh.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlblzngn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gttxmrwbt.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjataskfj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwctlqwuz.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gxiftoljk.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gcsmnfpww.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/glipcqqot.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvksvjfsa.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/geeciacbx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtlcafnb.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gbeckkass.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmahoeite.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ggtyrisgf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gslmptedh.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/ggpnmiiqs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyazjkik.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getykfgmy.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gsvxgyzmq.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfornxmka.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvasxpubg.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gvjolprwt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhggdsvq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmsjarso.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gykxjgkxa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpzcckoh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoylsqxf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjaaxfyy.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvmmplfzf.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnenvbbpn.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gosjwsrno.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gfgwgyqdv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/guclrntbq.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/glsvwljfk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsunsfwt.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gsuawlwww.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzhhpogq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxwzogsc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gzmantyxw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrmnxxss.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavhjudor.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvlesbig.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gykhgbcmx.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwniulacw.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmaazxykg.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gwrwyndxu.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gwuyxnjlo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gghpqghmr.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gbazijbgy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/glirzvafm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoyemmka.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwgmldgpl.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdfemnri.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gobvxatef.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ghihxlcpg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzplatdzn.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gismatbvg.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfflccwsb.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghupjbpeh.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbbjlytar.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grgzwyriz.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxvhwfgo.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/guiypmogn.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gnrrhvebt.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gacsiejks.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmnenryw.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gunpedgje.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnytxhsjl.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcoauxyz.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gilcszcqf.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gkhjwrhak.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmkzrree.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnucjygfo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gzjptbeww.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgwxmxeb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnohobnf.sHtML


<!-- 参考信息 -->