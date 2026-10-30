代发 wailian999

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtosdyrso.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeujydwr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnwtxfhd.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/giimjfpjz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/garnzuiaq.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfdxegotd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoewcwlp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gvddcuohi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxtjxcax.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleuprwcr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgpuhmtx.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gkbakvsqi.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/grupnldjh.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gebwlvtrb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfrolsko.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqnmebfi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjypsvkyx.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gibdnexmy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/guzeqfogz.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gckzkboab.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhnafycu.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkqixzgr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gixmvzdjk.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjmuijfmf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/guigsdiba.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gmjicjjxo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/goqxxbapy.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvqombht.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gvrjvxtti.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gcbrixrya.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpbninmn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gluxzbgtj.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaqwvgnw.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/glchzacls.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtajacjtc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkywjlusc.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/govoaysbu.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpctpytje.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqpmnxiq.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/glsbzxwhg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gatusdtav.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gdipdpuxr.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfwnerff.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtobzcsxy.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpeicqogd.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/ggxqsswuj.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gewqoaxca.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzxqesmt.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasehqgam.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gusatgwep.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvijhhxf.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggipgqjrd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guubqrhid.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gdjddjeyt.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grybkhygp.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbsrwurg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/ggxalkehc.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/giofvbxtc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjlonihe.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhxrffjb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvisfmrw.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/guguxcrmp.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gipypwlhe.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmqdxhow.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gbolbpfbn.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gllwulici.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnmnnlsps.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gidwmlasz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyryxaeye.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gdjkwzizf.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gqugoxmwk.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/ghwffizfv.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidiehbmq.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiucjlul.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmyxrzbm.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gapozawnr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvhyrcoq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/geclnzuka.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnnoqgzh.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdekmkrg.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbseyisyo.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzebygte.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gyyoyskqf.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gvffftjlr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gygqpdvpm.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmymmmdzu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxlybtqm.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/goftukxas.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gkwuxxoen.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gjcadyahv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisulgizh.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwleflwix.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdsxgvrf.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gsvpmxlzu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gimxfhobr.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gnfpqbwvk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghexubnkt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfacwubi.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqfzquuk.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkndkvdls.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gfcchljgk.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gfxbaxvcz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpvxwzybk.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgeikuzv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxnqmwyv.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsojkmihp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grlvnkewc.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvgrtpiah.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/granodxzj.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeuahjns.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdusdixm.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gflnzgvzn.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/glqbscgah.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/glkglryou.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqggpwsn.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gebnlfugg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkibcqopz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuquuonl.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gljptqurx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqkifqshz.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gistlfivq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuisktcn.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggasyzvkm.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtapawxg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqskitbqy.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gqnmegpus.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrfhxzno.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvknjcbe.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gkezpcbtm.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gtogqvzmy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpabyufh.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhbpxozs.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggyrlclof.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gepkqagsd.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkpylpno.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glztylaws.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/ggnzcieiq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmkxckgh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkidogzrc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gezcuzsru.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/guojvhnoz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocsfoduv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbbrfgnu.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxublfth.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/geflenqkh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gsgzntuwj.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gvnqlfbje.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwtdigxd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypvwtvsx.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gxhvrhoft.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsoehyaf.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gtbatzklw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gqvyzdsdk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidiumsho.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/glndkvpgm.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmrfgzcm.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggddfhwou.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmmjxahdv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gdequcwko.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/grpnqvzfv.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfifuegic.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gznzhxuaf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjfjhtin.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gveommgdv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/geihtfbak.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsbdwpse.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/giykepbgi.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gumxqydcb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gjkdyrbbl.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gassymlyw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxqyuwis.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/goozejdhq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeenlsjg.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/guaymbsyj.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gaviswlhq.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyolgqxq.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gucjrefsy.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gpcfahetb.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwynapzsz.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqtrsvfvi.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gfkcuoyfd.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gontxpthd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvzbinrm.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gctshmrns.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxyafene.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gtvujunbb.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwqzgzfi.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvggutqk.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/grgrbsuto.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaimuwojx.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxufnwzcf.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gortwyhiq.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gxwaitvmw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgcaizyb.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gppxrjzzf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkyfgncy.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvcnreyf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gseqyyyri.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlijbnbl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktqqzhxe.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyoerzml.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gltnrlxam.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxpjuitj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpfkebmr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/glvoraggh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gefmnyvft.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpbrcvpq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoklwvfk.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiwgajvs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkkxkgnj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzintxsu.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gooknxqmj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyplsonc.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gpbolxqhu.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/guqqrxjpc.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghrbwzplj.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gedhdeegw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gbkgzhvhb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrwuxzwy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmjjfnlli.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gslddphwn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxtalcgd.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmhbspxf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gfbbxztnb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcnpkifx.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gggpuwxzx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gibtbhpss.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gbydwgjht.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezqasytc.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwrhdufzx.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gysoetrzi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkocpmwlr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grisfhifu.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gnixoekzq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getjszeai.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnuseley.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzthunmn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpevuanu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ghdwnolfd.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gwikyfekz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkicgvefc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrkmjfos.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ghnzxsacm.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvwfmhkk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudepnhpj.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijyxzghd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gasksvhjm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gfgqsthgv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpqkussb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvrmqrcf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrqzubup.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghexmgslb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gplshlqlu.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gonnbyckx.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfmramtrd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkuvqlyw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkbchrdf.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gjgxkopwn.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gfxhyqdzt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gxulgtbpj.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhwmpide.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gweftmrgg.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gpzbbexoo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/giksumjfa.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmgukffx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfinbgdb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gipxpfymz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwsvbibwg.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gffdxqnlf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginozmkig.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeqfphqs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwjhvfbu.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gljseoqdg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gjxuszfpm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/ggxaysvyd.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzxlrzszj.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/guzxifext.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghvgxkwsf.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/glwpmzthu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gulzfvhyn.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gsnvvoiwh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggybjjpqx.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtmuskaa.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gzjikgfoh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdlhitcb.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glquhnukr.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbxhwqhj.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gxiblqnmb.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gylflfrmq.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gahixjsrq.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gapyiqoqg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntncmtzx.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjvuhhcj.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gorkhtamy.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gryzacntf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkkxttqm.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghbgvghmi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnlnleid.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gfieawlsh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgaffshj.sHtML


<!-- 参考信息 -->