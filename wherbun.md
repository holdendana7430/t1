代发 wailian999

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnnaofgwh.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gbmdmjdde.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuoammfz.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdfwdhuik.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxfjwrjdi.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gyobhuazc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvnoieumn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrlrbdcs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpfclycte.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gifjtnwyn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gobzbbbhv.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gixeheakn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/ggbjnktou.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/giluqdjbo.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gbknibmse.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbqxcspb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoemiqlf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatctpdzb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gnrnqbrig.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gicngvwoo.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxasmiftg.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/guhuctmfu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrifqvgs.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gxsyevjxe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/ghxnargpg.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllprsyaj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grarkenxo.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gtwnprdbj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqrpbwuw.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxumkjib.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbhancoh.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdoumfkpn.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoyqalek.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/goyxcdnsu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshuuteme.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjayqjbq.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gywcyfnaf.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqehlmgo.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gntsfxdaf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpibsdzb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnhwikda.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gixowbvyt.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvclvflwv.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpazwkbzg.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gzltdjlhe.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gatgbtznz.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpbkdjxed.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpzrtpfp.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyigzpdvj.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghippnyc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviuwprit.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjqdsfta.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjzreoliv.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkihefmkt.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guodhfgvt.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gpwblgdyc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gucuadzmc.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/glnfgzudq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqshnglw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucxutqzh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjewpzdl.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeqyppqc.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgpiunky.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeoeftdq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gurjssrfb.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpcdtjxo.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhtolkmc.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gixutzbwb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipwshkmy.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlfyfcwm.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gpfjuqiyt.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/guytqkobi.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/grfiqxqqu.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gurhveccq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwnszekm.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gktchpayg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gzckjvghu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gscponwtg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gqappjnzf.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gkgjdxblr.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gyhvqtusq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbqedfgj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gktqgjlrb.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/ggzdxtgxn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gyclfcvdn.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaygmoccv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbbuuyzz.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gspgxduor.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gkygddpzb.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/ggrdwnljo.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gjyxzsxnw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpccrbmh.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvmtjwyr.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gcwlsuhpa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqzyrgzz.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbjdffrh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrxutvjj.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gppezoshu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwmkzmcu.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grwckhlpz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gywydsvge.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/grbrrwurb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzzzbfsv.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gcxwzyyzr.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gtqvvaods.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gdipfghsn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gczlyqvga.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnobyort.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gmsaekble.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgmoxfbo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfbaesto.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/guwucofmt.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gziwmfhol.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouwaqtul.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyybgewbx.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gusyaepfv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grmkvhmse.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqorayfq.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gssjhzllf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcstfjybh.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyprhzbm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynoyullv.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwfmmhsrr.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gwftopdix.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmkyrllt.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnifdjcg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdeoqtmy.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gwfuauqwk.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtenkkkrk.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gopinofzt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoxnxsgy.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsxfbnfpt.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guphtaryk.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gejbucvlq.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/glbyhlqqc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gozfppfgc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gltocfrmp.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpylupfe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzgyzvsc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/godwmusfc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktlhxwht.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfvyenbx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdzkywem.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqzqudsh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gsirpjiqk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ggpqecsup.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjshslgny.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdksgzxc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykyzosei.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhkggkqx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gflxvodvp.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gipuwzxsd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmzjlzxk.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gttdoathl.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gvpczvceu.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdmefgdz.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gsymeupux.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gfediwcix.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grieexjmj.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkaavxwi.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/glwrokwxl.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/glqqvzheq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlkizyuk.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/glhcjpfys.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhoryryl.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyekbgtwm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixabflzx.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gbzgjslrj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gufsnrmpj.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gegrrjuka.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/ghewqgaiz.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gilviqnlr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gexrjccbn.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/geyhzlokf.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gfwxicaag.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvpasqnp.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gagzwtyzf.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/glomzfqxx.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgvjygwc.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guwtrmqpk.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/grxszlxuw.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgtctawg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyavplxtf.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gyrcbvbhz.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdcsbuji.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeoxrxnd.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlzgqntz.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqdlersq.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfteycti.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkplfvlwj.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gnasnypmk.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gbfwomrra.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcwnsvqz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/guilatofl.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gfymyrwsx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrhnzgde.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtgevpvh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghgpdjqdn.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gtylkwdbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gieriaucv.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gpgrlotbv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/glzsklxkk.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdrniueo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnjhdrff.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyjalxsy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/ggooxhidx.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiiamign.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqahnzpqz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gltmkunnx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gofdiwwvy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmstfwze.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdnbbovw.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gkboyckre.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvlswmzc.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyqoghsg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoftdagf.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gadppxnvs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gcniyvbjh.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gdwsmdrij.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glwxphyuv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/genwjaoni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gduaecwzx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gldjampxx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gzbgfuxbw.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgydslsv.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjxxfamh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gbbdgeycq.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gxiznmeqf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtpdmipa.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmjgfzhcq.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkjhvzkrl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazxkqycx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnomkwolb.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gfpxretbb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gdbknieox.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpgvaokv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqccaxbjh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ginfvlnop.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gcfcxqnsn.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxswwzuk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsxvmzacl.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gusybiclo.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gledblfjh.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkegdjnf.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gvajcibqi.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/ggzpgmlje.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gnjqcojft.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gaflnfphu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzmcwmhf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggltvyfyu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/giwmafgam.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwapptkiv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gautpvnzl.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwwohulai.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggacphvso.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gpzlfmvgu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyoddtln.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gtfddddbv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgnbawbv.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gshygchyr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gaapdtjxy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/grdgfftnq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gluhfznng.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjhaouva.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnwgjegy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gopmdoxxm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gltqeevsu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaebsihss.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmolvnzb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gajwirxoh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwymhldey.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gibondlwj.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/ghofhassd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gbausissj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/giapgjbry.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/goxvhbymd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gwocmsxus.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsmtgerl.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjjuxkil.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhrjakti.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gsuwpphxg.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gpttdjlhh.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtzvjfnz.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/giyytjiff.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gzmvxcfck.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gndwmncav.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gnzshjzlf.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gsfaetuyx.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gznfkzyso.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gnwqwerwy.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gurgieksk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwugagepw.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gylqufkuu.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafzdmyeg.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvppslzm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwqwysbc.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/grkvuwzki.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gozmvfchw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcioogpy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtopdrqck.sHtML


<!-- 参考信息 -->