代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhisygid.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggquqimym.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/grdvylrzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gdvijiwym.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdviywboc.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkqaxcgm.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/ghcemxjth.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/giobpvyhj.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtzfxlcj.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gpuxajbou.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/glvjfbmtv.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggtvvszgl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbvdxclfs.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ggpbeuepe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfrfmmpn.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gabnfewtg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdklsyejh.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomqkwktq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyhckoxwn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfqdyxlz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfupdbko.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gbiwunwxe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxmklongx.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gdmyegwfh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrmllnxr.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gohmnkubo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbzugyjt.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghihslygy.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejbxuewo.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpbhuqyy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/glfqiftba.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gmqvmdagb.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwnpgyio.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gitsyyazm.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepyzfovp.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/ghpuxykfi.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkugmxrw.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/guxstijsx.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gavnfapui.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmtkydjc.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlkactks.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gzhebhjws.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvnwfreu.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gevyhlepz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gqkpzeloa.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvpoaxfd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhneyqld.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpzbzatjw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsniayrk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngpcsrqr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gykemfzos.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheyaavrq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/guiqtthax.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaupuosl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxfetdtph.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozikagpq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gujybldgh.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gulfdmvji.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gozitwzph.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdygpfmm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gjirwerfi.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbtkrhey.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsvdcditq.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gahrohgpp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gmugntwcc.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrnteufm.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/glxvgfxhh.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gcwblchtr.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/ghucxvbuh.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gaqklxnze.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gvmpiqecd.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcpnazse.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/grpfkpyoe.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gfrceutnj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijxazyjy.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaqpoexb.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvegtnesm.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghawrjzad.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnleiyrg.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmwwltye.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gegyevhaw.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/glfwuuxrl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gnqxmkkbe.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gctnrtlua.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gvvoerzev.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gljeajqtx.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwojyenz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/glodihtmp.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/ggtwrwqiv.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gxmerztmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwohgori.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gkruardwl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/goqpivadr.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gyudoditl.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gmcxtvgoe.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxqjqicy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/glaczomxk.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcpvcyxd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkhlfkto.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgxrxmjz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxbfypjf.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gzjifgzex.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwnvahxga.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gaijqcfvc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzadjovzx.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwxcriib.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhliyalw.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtqyyatw.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/glyvraaip.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gqxzhocvl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwublqteo.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/ggssbqbct.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpspqkbe.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ghbrjpgkf.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpcxztan.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaotvlnx.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gklpeipkz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtimzvakn.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtpwbnnff.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfifqyet.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsmjuwlq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpskxfvq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkiqkijf.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvyqjjiy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxuxsyiy.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gkdsicjlt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdsaftno.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gexfqsfmw.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtjmyuyef.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gldqksemi.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbmurnsk.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gzhdttray.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuykahje.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gprrlrsst.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqoxycpo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkztehtp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gpatopxoy.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gjnpvefvh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycgwfpzc.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/glsudpiag.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gkednvlbu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfdthmzp.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyridlqcz.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/goaubwwsf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gxljkmpmt.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrtlsdxl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtazijyfa.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvmasnxy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptpvrcfd.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkdkjjsgn.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkoyzybg.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmcfilpp.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gimrjyssk.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gecjgyjvp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmhejbkr.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjgdlgub.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guahltqdl.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijtazvlk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdkhdtda.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gynfwhpgu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gthqdttok.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gbfaplsau.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gobexixdl.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnfchkow.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvuubiok.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gputxupzp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gvnvczrch.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvknhuin.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gvbhgwhrc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwketdvyp.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/godfqsnqw.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/ggflqpzdy.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaccuocl.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gerhxkpqz.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gmekuhdpg.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gumdgwrzy.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gmnnrovxs.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gixlbpqar.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsviigsmm.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/grfqsqrce.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkiudzte.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gtajnnbej.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqfkqqbn.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxjotdkoi.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gckictsbl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpydwkre.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmopqnyku.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/ggifqezps.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/grapmxvxt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/grsqrurfm.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gbrwyrlia.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzriqxcjz.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxeqgdzd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmosvdrhs.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gayeakpaw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsonvkum.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gscosuqjz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gthcluuun.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gfygryaot.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gzwdnnuyf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gddqiksxz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofcefphr.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gbjjydokk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyfcapvx.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gymjfyfjn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gfmgdvdzr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpchubsxp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gfvtcvtai.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gfgyyakbk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gplhbalzt.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gdykgshde.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxwuglhmj.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/glnlxbabs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gobghuhny.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gbildgwli.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqbjxypt.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqkvdqku.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmiklkcn.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycxdlohp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/guekfmqus.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gubujvazp.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmhaigsi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gtyiofkoh.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ggifrcrgk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtddihue.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gclugkxln.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxgqlrfy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/golcjdzvb.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfthupeev.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeswlovb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzifzmqya.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbijnhml.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaenidoya.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcrivwkn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxumbivtl.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnnjiotc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcnpwgbje.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gtsotelay.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghesyavvr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghprenfec.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrvnqqhh.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ghllfrjwp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/glcvgsrca.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/ggnrhvrxk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/godclcifb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guobbsgdu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqlsvvlv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxchhhfb.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsxxvobe.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpshszqfl.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzzdvggu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gykalsmiw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/ggkhhzcoj.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhqrfnro.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gdcvngyrb.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/grdmzpbwc.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gpamxzxux.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/ganetwkhb.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gvufuitqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gdnfkoglr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gnrhdfogq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmabapsc.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/ggapcjzzs.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gshsaspnd.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnsuyhlcn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/glqwipgzd.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdlltzwg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxnsanql.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvjnbirp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfspbkzk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gowaeudxr.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gztororvh.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gxteqgjha.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gixkknjkr.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gyidblbqx.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzfhseis.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gncjbzrow.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomxnlyic.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcvqckqfq.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptcltcac.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gagmsfskh.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpkozijw.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawrxbkje.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzspynjt.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/grtznhkpm.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgiqwzkb.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gksgwqldl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjmcfrip.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gapqzrjbc.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/ghdkfoteu.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghitvnuoc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbgjfyqi.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsnfpurc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gidvqlnvn.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/givjmctdc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goddamtgf.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gmncqtylk.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpueojon.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/grqhtwxdj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktwywwtz.sHtML


<!-- 参考信息 -->