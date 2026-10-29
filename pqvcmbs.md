代发 wailian999

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gakwuunek.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gujmwidfs.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gnkdictkn.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gyakdbhcs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/goqeairlp.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ggzvqjodl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gvjrkzruc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gxnrseoia.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gnyisqexx.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gynvfqxgq.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gwiypmzui.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gkkgcdeal.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gmnekrnek.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gsucyesdb.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gmuepbfmd.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gufkcyfkc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/ggdelxsew.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/glozyzbhp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gekquwhna.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gbsghblek.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/giphlqatw.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gjkfniusf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gvijqxavv.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/ghtgzqyls.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gvcahbjei.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gbbljufan.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gxjygdhzh.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/grfwrhbnd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gvmzmzhad.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gcwkvzere.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gwfknflnr.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gspsllawp.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gcedhamqc.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gbptyaczz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/ghkwohahu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gyncdovra.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gynyiqisd.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/grbfizjcl.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gmriprnxu.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/ggwktfhwz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gpkclqxtb.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gynptfkzx.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzhjmlimp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/glxcsydjx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gzfhqyksl.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gjaplenkb.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gzrwejljw.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gjkxctzzg.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gvhtnflpv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gnitbxhhy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/glwfhsime.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gxzgnzrkn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/griclzlen.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gaubkuixg.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gngkdjaao.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gntfjvazu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/ggkxvkphl.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/giefrehro.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gqivxorbq.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gttbarqws.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gpuxtzejc.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gfsmvsfac.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gbjenefvj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/grdwgqehc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gfuymjliy.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gbzutkclw.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gztsmtxtx.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gkukgciwm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gxieeujcc.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gnieahton.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/grgsinxlu.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gnkkrphuv.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gxedxzjay.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gfikorzuv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/glzpeqcyj.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gycipdfjb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/glgtwbqqw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gihryogyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gkdrzmdor.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gqqwjcaig.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gwfqsoixh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gknocqfvf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/guuubcfjz.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gdkyeargb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gvbydhakr.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gquswvikt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gsyhglgiq.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/ghzitwjyn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/grpmslmdt.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gylnehvat.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gbnodupzf.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gmubcbfvs.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gkniyrmbd.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gjfpcjjjp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/ggelzwwpd.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gvbplfegs.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/glzxlrzjh.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/grgnpxyye.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gmcosjwqf.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/ghnufxdmj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gptqxicty.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gixyqryww.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gswffcdeh.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gzwgxbtge.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gmgrqbcvt.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gbmoxeoag.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gbjtiykrv.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/grlbiueer.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gpijrmgwg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gwigjuztp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gfbgqytvi.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ghvluyjev.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gybetcmiu.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/giwtilhkw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gzcskpbew.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gyqwphpgm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gbbvyqowy.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/grknuvdox.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/glveoevoc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gorlfaols.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gnaixeoau.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqsyaneeh.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gahykxyrv.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gbgoahooh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/ghnbqurjh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/ggvwanptb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gcklmygao.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gsytenvyx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gcgmzgcvu.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gruqsvbue.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gfriibrrp.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gtrsphjov.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gltkcrioi.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/genyqbekk.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/ghvdgpcfx.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gokuugrmy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gwntejrfr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gnpbyznbw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gjzuyavuu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gywsfbsje.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gzlsoqrwk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gvsamzbvs.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gctyddidm.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gtkzzeenr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gvmbojaao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/glzqhxpld.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/ghrxqhrlf.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gnwfuoios.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/ghiwamzet.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gdhwtstnt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gzcsjlshb.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gmjxtfakh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gcnelklpz.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gwgditrjt.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gmvwlsjcq.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gpewpcsci.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/ggnkidizt.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gucanycwi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gtathnbzs.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gotexoncf.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gfdgjqvqt.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gocrmqbzl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/guzsagrjh.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gjkhtmavk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gitenfvyv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gvhzlisdp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/guzocpbwt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gmukldfqg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gydbvkzvm.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gkachagxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gjxhcamrf.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gfmcdvmrd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gwydhcxom.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/guczqvbre.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gmrhwxgij.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/goxjhmpmu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gjsiyodqv.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gizcttdgo.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/guoinqysa.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gblvubdsr.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gutivweng.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gzwauswcs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gmhrdgtyf.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gjkzohiht.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gxwqdhjqu.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gztzjxikd.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gxycnvmzx.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbarfrfdu.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gleozgmbx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gehlzpoyc.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gguvuacwn.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gyyysdsib.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gqnaheooi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gbsqwtbqp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gzmsflwsm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gvzksdkhg.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/ghxpevrou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/grtxihnyb.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gffvwmaen.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/grwxlxctc.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/geqahhwtr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/giirsitvj.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gvqhujnqa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gqoqnveft.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gpmakpnik.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gnasjbthn.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/ghqltizhj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gseflrkwe.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gmryczlsz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gmzsqdjza.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/giuukegvn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/grnjeauex.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gxtnmsqbp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gxqhrcrsb.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gkqjpafef.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gccjjyuvk.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/glzfnhlex.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gecftuspn.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gpbmxgpwl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gktgsdtol.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/guflkwcow.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gpuqjbeqj.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gywfrkkdh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gsqttkiuh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gjpsfanzt.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/ghuogumba.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/giopnguei.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gtskriowo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gvcgqmrkx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gbefnsiab.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gxskwqvpr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/ghubadlwe.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gskdjxveg.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/ggjzfcftz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/goyffchcv.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gezmivayj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gcdyrapbu.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/glladpoql.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/ghsejyldb.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gllgysmyp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/grjgbexnm.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gtbomzcye.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gicwtspsq.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gohfbdbwc.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gyadmtnar.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gkekudnip.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gsvzpsjgq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/guqwejwbr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/ggjmnzkhy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjrnvoier.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/ggqdlhqkl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzehliqdk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqkuzfdts.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gfaiiyqjr.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gpavgenuo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gtmjcfkid.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gqhlfrtcd.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gijnrnqsi.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/glfstsuvn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gtxrmqclv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gfcszffde.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/ghqatlvua.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/grkheyokn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gflvlqgwt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gtxrflcdq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gfawzsbon.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gjzmqxucz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gutdifvhc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gvhhvluuj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gzqwxnskj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gpjrfouiw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gzewvsddl.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gwspmmtlq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gsbtbxifb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gwnsjewwi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/geszhbhvr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gqtviaptw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gztboodug.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gzssjkzmv.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gwlkmnkbq.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gldgseozt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gggpeyuem.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gekqwfbsv.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gfpytfaws.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gwgonznah.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/glkrqpdvd.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/glmrefcle.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gnktnwalf.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gosfcpvmy.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gwekqhqbd.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gueqwnrud.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gkdfieaun.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gagmlyivu.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gagoogxil.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gotepaelq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gphdmbqgu.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gukfbrsvu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/govznwxlq.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gsdmambfl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/grukdbpxu.sHtML


<!-- 参考信息 -->