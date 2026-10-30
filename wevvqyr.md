代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gibstifep.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gcwwzkwjj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcjdfhzi.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gerqoctbh.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grdbwjval.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/geltqyhae.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbxgveza.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaskwsps.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gsatwfaqm.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqokcwas.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gyztdcmzd.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gquoyymgv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtwwoggf.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gmeumbffj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gfsefgbhx.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbifcutmf.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcylxwfjm.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gzomapmak.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfkvhwgg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/grefnsytc.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvflfqzet.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gppsczjfm.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikuinsgt.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gimxyrlcc.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/goqegdrwo.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gleceigft.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gndblnowi.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goifgznyl.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwblbuich.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gzwcfjyab.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gqspiwsya.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gbxmcubzx.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gbmnasjeo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gsurcbqrl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gczsogfzf.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcqmmrlx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxwdovhy.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/geucmfsau.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxplrtkuq.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gixkvjciv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkbeucgj.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybtljlnq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdigjuho.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjmvlxox.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzijzimf.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrztxxqn.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqvtqiegd.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmffkert.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfqgbwyc.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoecqdsr.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/giyriapob.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdxtbsha.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgapsmvd.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbtsdovx.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gimqqhqfr.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxslvket.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/ggbhyuboj.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbewdjqla.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gnheslcqs.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwsextdm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gmtipbpra.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/griunizpy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gwggdnvde.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpslkwtec.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomuhlhyt.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxkookon.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gehgzqxuk.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gbadopoio.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/grnxztsyb.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gyzgxfehs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gmcnakjto.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvskzfuuv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gleqqplqj.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gawgdbavz.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/grswkjqqn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjyqcnee.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gwaxohhiw.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gqkealeyu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glkxqrdav.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqajazsmq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/goyhwpmcc.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gcglietzy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpojmush.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gwiutongx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/guosjjyld.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkbpmxdf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gouxayvan.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/guypaxlsn.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gynujkkqq.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkfxbtgj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzdhtfcrd.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsevshyhq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiwsaatk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbglwzwsa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrhguvfk.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gvocipbln.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymrkulvx.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gnddqknnd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmkjsyvok.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuuronud.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsqvticfe.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhlfugbm.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/glemxnmxz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfppqrqlz.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gtnwjckvn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrcnxzte.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruznaeti.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gycrnmurj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaugezlne.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyltdbkd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqopzdxp.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gfomvrqzz.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gxokihyri.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gmgtjfrsk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gclhxnmbh.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrmlwytl.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmoljfpe.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjncnyzlj.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gwvuchgjt.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/glofahslj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gzbkzfexo.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gysdwjisg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrtudkix.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gtptacxwg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gsqpghrmc.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gnitltttj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyndnjopa.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gklkazgpa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gowcxpnvt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfxfznpz.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmezwweg.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gezfonedu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwvrjvbf.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfypjarm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gypfeopjl.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuscemqe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gcopqcenp.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/glbbtimve.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcmzckoo.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrdyaazg.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gghjjyoje.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gqpnuqalo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnrazgbe.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/goxxwwwiq.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gcbjigwji.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoifytii.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gjmdlcjlr.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuazjlaw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemjbgcks.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbwuaytbc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gemdzyoeh.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gcpdzqboh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbbnisqp.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gjbpqzluv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzrmojqv.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gdltaywrv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssacwfsa.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigdqssse.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gilxyrsea.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeyiohio.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/glcgpeyby.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkcgtkkm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocbyugge.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxcfadmo.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gprngykuo.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqyazrow.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/glxyecxmp.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gclmfvgkj.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyejvjuo.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyouprru.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gjwfhtysb.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gyknvjnao.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzuibrjz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpalbcvdi.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gvlrvjnrr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gigqvtxny.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/grqhnkwpn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gufufgtdo.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gjeftiapl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczihpgpg.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gaflzgjut.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvtzewcy.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gaxbukrrb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gchqlyzxw.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxubdwxh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzajilzda.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gazzdnkhj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhgzergd.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grjtehncf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/grikcvvzp.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagvbnlur.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/garftwipm.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihvwctgs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfordsvqc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/ginvxuivt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurdsyuve.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikrzslmg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gkkwuqlxg.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrtcbltr.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/guspxitsg.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gocdbcnyu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllyjdqcr.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrcmgcqc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzugmyzfb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzcajcpu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/guehumjbq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdytshhtu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gviqhahil.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gmxldmnnr.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqztktwu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpazjemb.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvxovpcpu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvenbxha.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwagjocgr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqijiffg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gcybbptoy.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/goalycezp.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/grognkopn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gukemyvmf.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/glupfzpwz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzsbqmno.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnmsecyx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiqczoea.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmiakuss.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhffwqlo.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghvgweaxk.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfzjhrnb.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gjdwqmxsb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoezxtoi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxsarsdx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gbvaejvsw.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnitlucdw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/goiiudcam.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpbawwvzq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxsvpnor.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfskmxrd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlneihfr.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gehpqfyvg.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gerthftpd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkujeenha.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gznzvaqeq.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gyrwfdyzl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/guqvtkwix.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gtpxulnuy.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gmvdiqukn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtvnaktv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfwbgtij.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/ggakgmjwg.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/guxtygsjc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtgabavg.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvdmtrdt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwrolyfh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqhenpfe.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqlliytq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgtuhjkj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gxtjshdik.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gwmqtcjpx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbapeebd.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gkqxyxskc.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gzjecacga.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcplsmvso.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmshtszy.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaszstzj.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbieouzj.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gfbthkcqf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiyklrkj.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdmfteeam.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gtgtzidrq.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gehjwztik.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghlvdfxay.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/geisdsuxx.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gtdlljxvk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhghipih.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gkbgertmr.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/grydpjfvg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnnbtlik.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlnjfepg.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsubvaoj.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gqevehwjb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnwqukrau.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtrtdlagc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gmvmkadby.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gfususzir.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gavuihqnx.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gdixxvlzj.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gttzouzqa.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajfzqnmu.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnelcjfto.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gaixqjilw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/guhjrybnp.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnjzuxov.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdykyixlk.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gqqgnnrbh.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/glpskbvnh.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimqvueif.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gxbhpehsv.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqnsyjzn.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiubktse.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgssfphl.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyizycmd.sHtML


<!-- 参考信息 -->