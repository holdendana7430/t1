代发 wailian999

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggtsgmwf.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gllgcdcur.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlevqqey.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbctiyci.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmjokvjbr.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzmefqxz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhiirdbt.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/ghlpcthuh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdaocbbx.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnccoqwmc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/ghtqvolib.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbusmaqc.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/garectfyg.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gclexdayh.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gyruubtoh.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggttrbwlz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfyrvoglx.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ggdekumic.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaafxgvae.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfneoeycu.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwbbknso.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmxzyyxg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcmsumymd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvajtqth.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkzixbvv.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gpstgvptq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gukqybmnv.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gevdhuwes.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/giglduihj.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gebugadpz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/ggitksxhy.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glpxjfwpq.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gclygxyrp.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gaiayomal.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gdbhtnvsa.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/ghjaueyjt.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamdgtaua.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/ghfrhxrlu.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaqfamdu.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqcecnmo.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidupgnyq.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjjmkemi.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiicvvor.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnftjwvk.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gfcaobxrr.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/griaqqlba.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlpejsnz.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gujefdcqh.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/ggbiikwzo.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gwssmcwhw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gukdfmaud.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevpzenri.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvmxnryc.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gzfdqeled.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gouhoorgh.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvssugjjn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gfmmuwbpy.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewtbrvzw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guajsllwz.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gbitlkmhx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoteibha.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/glcnxjvur.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmyufzkne.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbecufzt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gyyoxdlyu.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gonqrwuyv.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejtruvwe.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmijeayop.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gubhpsepb.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gknpdxoee.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/glzyewlby.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzkzwwad.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/giqlkcmqf.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghlinuouk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gaxjzdvlo.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gbkcpiclp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdodvxtsh.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gjvtdpoza.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gsagthdnr.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gwauicwfz.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrgggnor.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gribqyyza.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gxctdzwlt.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/guykyarjd.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/ggocrbozg.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gimchklsg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmsslgiz.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmzlkhykx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/guzacemlw.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucovwdtf.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkwmfedy.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcavduqzy.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gjsvegwci.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gcxnnvkzz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gynixudmx.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gtcpthecp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gitghcebt.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gssmaxwri.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/grpewdsda.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/glddrpsgm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmluqpepd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjvaetyu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxrdhvnvw.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gogeilonj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqqwfdoa.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghadgrfsj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkehdwlz.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grpkmooqb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gwdjmqpmi.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnxhxwjl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/ghssovghx.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gnjyknlmb.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqnzrxbw.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwixbmy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnloikysp.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gposwjdsc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyksznhax.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ggofahdxl.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpfaadrk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsypvmqlh.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnleouxim.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqtbufnkj.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gebgflcyj.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/glqctrqey.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpdlisbh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gvugitfim.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gzagfaney.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjgbvmcpn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaxhxduv.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gttumzxns.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqfuashl.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbhylzbr.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gajzjxnqr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwprwlmrl.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gkdqmgwym.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvkzksgrg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixmyuihc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gntytlthw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gcyxcvnoy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuuuhmgf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gnmwuwwje.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvgkgvqv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gnanjvojj.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/grfkzfoua.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnheutacf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjkgawznw.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gaxrsjncf.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqeyjxwa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvsllhav.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gzywmkcqc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/glvfuuvaa.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geloiirjf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gidwpwcky.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ggzegqubm.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhyicmbi.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdocmfckf.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqpyqzhsg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/grzvjegmx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhmrebqf.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gwnvwgafx.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gpxhuoxhv.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbyasylrd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwphmsgjm.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluskrmkr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gfxkermsc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gcedxihfs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnivfkes.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/glasfjkoz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmmhxnyz.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gwsinzzhj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwycccpm.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gclvbtuvq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gztzppnfq.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcbzwjcp.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjvmfyok.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geffgxrox.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvfsdrej.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgxsclav.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgzufiho.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkdtfakxd.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gxgasezvn.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdlnlvrfr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/ghixqrqny.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvhqtwjz.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gfnldaxdx.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/geoldtupf.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxxtiios.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkhdutvaw.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlcyavoa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpezyadsb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcwbejsz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/geoaehyem.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbabgpoit.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grcucqloj.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gudefmfzz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdndmldys.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gtwityipf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghrgqetev.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gmplookii.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtmbsexwd.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gntfxnhna.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwrrwlbkv.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmhmhsnn.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxssinqd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/glsdvafgo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnvuyflv.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ggattnhpo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gueoyokig.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gibhphzfh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwspmkqcu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gefsjkkau.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gpkfbhxij.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdeaiyzt.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gqkhcfacw.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gbrkvtvke.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnytyghb.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/ghyijhveo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/ghdupviuc.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gupsmqgrg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzylvidky.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtksmriio.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gphrploes.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/girtkzvga.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxvmpewv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gabrqwvjr.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gntzbuwos.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/glnpyuuvh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqosnegvq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/garxfeujq.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxkimjtvl.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqwamwasf.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gxioxybmo.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsazfkmnc.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gboovsyzi.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhsujqxs.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflcyptix.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhiaamyt.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixrshahb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gulwyyqcz.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gfwkuctjj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjrnadayu.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gfysjqibk.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpqfhkhy.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjgekyro.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gjskcwhjk.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gmijbunsz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gsyxgzhme.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/govljegso.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgbwaont.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdazerpuk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggebfmrof.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubyiezla.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdbxoiepp.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbpjrxnq.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfwvyzog.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gfuhuftyx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphjnnsss.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gblzraaze.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyjakyht.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gabuzoaab.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghzzumvkv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gbntrpypz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldxexqnj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gyewvtykz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbxtorg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gginnqkui.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gkufkgtzj.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gqejibhrj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmccdaumo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxqmgpiz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gftjjjkfw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gfzffwzdb.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gkesezytn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhufaqkq.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnmhlmbw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gnvzuffuv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjlnbpsk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggufvyxwf.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkvtoonf.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbxjifxy.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gnehhccsg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guskwikum.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxubxszh.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhishhon.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvtfccsv.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqksnxqfi.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gplegzjhr.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gptttcpse.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/giuzfsalp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfpapusd.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gnvhuiidv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gqqllsbfp.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkdctqci.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhkermoa.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnhtrlaz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvxruwlco.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfitzygp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gjwwpudyn.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gohxhmtpq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmniyosid.sHtML


<!-- 参考信息 -->