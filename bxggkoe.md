代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqctwtkly.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmyfijjjo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gibydaxoi.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqpluisa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgqypuvc.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsttgqxf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gvluwfqxy.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guacpozqs.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gxxwitcsu.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoqelsuh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/guylwpjoe.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdoublynt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqaompblt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmupkjck.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gujsyfjik.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyoudejix.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxpfwdmjm.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gbgutsylj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grifwjhnq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpnjnden.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gaesdhbpc.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiorsozv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gmzsnleta.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjolrrby.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gxrjyvzrk.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqwwjvmz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrdsggrq.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbkknnqly.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtefyfbps.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gkpsefrum.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gmojwhahl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbwcthaq.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gbkasoltr.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/geyfxfghm.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gefphaabz.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdlpgmvq.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfnedpmi.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpnuofxa.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouimhofi.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyiidoam.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqzgxuxb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysqmpfnu.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gxcujbsmf.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gsydrxvbx.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdbfwmtp.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gdrxfqbgm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gkdulispt.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/geoxgminh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gasbndykw.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrzgiqpa.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmywmivh.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gmyzouhvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gqighenlo.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoallcck.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guvztlhqo.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/glcfmmiol.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdnatvdn.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gjppssfth.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhakkssp.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gghtktahm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gspyvybpc.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcclhtfbl.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazfvzdxx.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwwutjfg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/grpsrqsnc.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjlyvlfn.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/ggzxnzoeb.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjzppdye.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/glpcrture.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giazembyu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gpijhtkdh.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gujjwxriw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gnjwougjz.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ghayxutqs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgiqjpze.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnqzhhtt.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlbwponn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gynzeopgz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjjtgndw.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfqatutr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuzukvna.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gddpjmlaz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gymnkbjet.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gixepljbf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/glfjpedzn.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmmyjxli.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvswtlpb.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gzbefhymb.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gpjwdswsw.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gkparnxme.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabcxdyws.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gsddjtzsp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/grvzlagcm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwagooqs.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqblndbq.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghblrhggr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gifgpnjaf.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/geymzuxcg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihqcehpg.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrkhhehd.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghszzwisr.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavxhuqrv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtacbkknw.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzzghcoq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmlerocf.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzaoisyqz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gppvswyfo.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gonrskjqr.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxqlxttt.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gumphozpc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnjgzwqav.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/geayavzdv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gufyzevxz.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbxoulxg.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gsflqdfmk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gaembrrle.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwcagtcu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gztlrukhn.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgeigavq.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/glmezusly.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqwcfdhkl.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpzyuufw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gouilhoub.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godoogvle.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjcleggy.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gjlgqzckz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnmuzrtu.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggsdropot.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gosykkoho.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkufjbfss.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzbakspv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gqainuddj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gwbdkmqij.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/grpenlchd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvchmyfxm.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/garkvwwez.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gelvfrikv.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfblepsi.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gedsdpmma.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgcrnbkd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvxvxkjv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gyewhbnsg.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdkloiac.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/genkyjrzh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/grnsrhhnd.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/guqmuhynb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gqjmwnpgo.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghujhymkk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groehvjmw.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/galwhzhwy.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gugfhuvyg.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gqrbovzro.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwwfpkyv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/galgjmbzq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geltymwjw.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gshesnxmn.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqslobmd.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvdyvzurq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbceifzc.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gugifhsks.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gksxmckjq.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gfapdsebp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gjmhhctkm.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gogngtdgh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gujsflcaa.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gzqbtaspa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gpahbcbqh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicfehnxw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gotihojkx.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gvnhidqse.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gxyqvnwgm.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gcvepkqdq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwflrzogy.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhqagens.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gkbrrdvgp.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxqdwyat.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gtlpyqagx.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghydjnhsu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbixsuof.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gusopuabd.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnssqiib.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/guwynwsnc.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gzrcmobgr.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaueokbsg.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gkyxtshos.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtfimxzvk.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasjvznet.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gltdrlrsj.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gfbnfylxw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gizhxages.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxqleqvr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gowldncgy.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/giodbhtdx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gddlhaswn.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gvnzrptep.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gsgkvgakt.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gibfkxtvz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/goiwgqeya.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqlvlxtb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gltmtpict.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmadiuth.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gozlgxako.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gmcifsmaq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxkjlxko.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfvzbuhz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuawjjwm.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnlfwqfat.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gqdhhvcju.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gzllvjczu.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gtuimvcct.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymxlsdde.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrvzbadi.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuejvzzx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gpxeusytq.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrzdueky.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/golchhrri.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/godxoofwh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyxghxiwf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbzhfqpy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyxjaxna.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmayljlof.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyvxkyte.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcthmcdof.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gcusmxxzu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gfuseaxpw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnigjcjln.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjwpgpsb.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gcdpjkkhp.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gapeskxbb.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gjvucotkq.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmytreqdz.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsjqnymz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gtbavhfso.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmrsmimy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/giwserrqw.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gjigqcilh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbmilbgk.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gvjaehlim.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gveagkodl.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/ghbbaoxyu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/guvqafame.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjbwaypq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/guyepmasc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmnshjcnq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhqfhfmp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiojjyss.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/giyrdyeop.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glfdlxotu.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcdzcgzu.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdkglyhem.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzljseek.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gvklbdmlg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gjtapohlt.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdktyrvw.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/ghhcwtjqt.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvkmgdsi.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gifaxcbul.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gxcnlmsbt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gojwpippy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwxjiopr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gbobntemi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gexnzvtmv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwekloyx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfucqkde.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyxhvtrf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/ggrtzgupz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmvwqgqpg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gloqtptps.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gickvxpdw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gwxlxgfxe.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/geonhopnp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqpdcfmv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsnicuqc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganpqkimc.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxdroaikk.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyjhfmlr.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiqggoac.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdpwjrbs.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnyfqock.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gcufczjjh.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmmhedms.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrfzlknh.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ghtmbqowy.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcklizyph.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/giqwnhtio.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gdwvgsvkw.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/grcyzjxgu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqvpxecf.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gharxzwqa.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gkplodsuq.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gneoouknb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpvafwex.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gehgcdnoo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwezkmoby.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gddgrgatk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjemscctl.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gntazippt.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gxkyfqbod.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gqbmluhks.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmkcysgj.sHtML


<!-- 参考信息 -->