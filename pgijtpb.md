代发 wailian999

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gaqhruyio.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gureqdzyg.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/ghpudrldk.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gvgzwuvoc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gtxskchyd.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ghbtqicqz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gqlyhmmzh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/ggguruyfn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gjxbmeyle.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/ghpngxaap.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gnroyyqdr.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gkybrulnw.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gshmpuurl.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gtzwcypji.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gabdzldmy.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/giryhlnid.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gzbfxdzxs.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gpwrmejky.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gtwwbcmsl.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gyqaovuvc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gnmmyrvnk.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/ghkioxmaq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gjmrboblv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gtpuvxgsz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gigcnbjtl.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gmszesfee.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gfgzebhuv.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/glwdrlwgs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gmruytfpw.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gswndqltr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gtnuoyzlw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/glwuqwmtv.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gkpekhabd.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gsumuklpv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/giivopjhi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gvjcjxxlp.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gpmyueufh.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gtljeinit.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/ginlalets.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gnyyhilfc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gyeyagfav.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gwqmpguoa.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gkkyphbnd.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gzplaixaq.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gozlauiia.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gkqzugnot.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gjzemumoo.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gdnyomxfm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gontoxcsk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gklfmapcd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gicdrwgqd.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/godoubobq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gatxpsoab.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/giodnnjlz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/goercshbj.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gqopjpbhm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gmvbtiaqa.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/glyfbsskh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gsndrkzxg.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gwengwsca.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gmlaqawqm.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/ghccolspd.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gvvhpdebq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gxwllaoij.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gfwctajpw.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/guwjegzlc.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gxpzxpbxt.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gwbropeic.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gzocqgtpu.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gauxqkxqh.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gmehonely.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gifflooji.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gbxnhsqfj.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gdeccfmsz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gaznbxnev.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gshiktifl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gtoayqwef.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gzafexlip.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gkdgubodq.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/glzmmowzz.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gqiedmrdw.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/grnsxqrvo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gxdyltqcq.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gmdkbgzuk.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gpijzdnfr.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gjocucpxw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gzibnspwj.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gyqalvxgn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gxyvbysrp.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gxzuhirum.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gbokzjzow.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gedxmakat.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gbgguqgjz.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/goezmeqfo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gipqihpwl.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gnbeswqnc.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gzprloqmw.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gdedmqgqi.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gctpjizbo.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gywuvluza.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gtcgzcfbe.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gsjghqhpi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gfptjlzmr.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gfurpktzx.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gpxlhgnem.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gttvracni.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gzqyxbhkk.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gckkvqaqz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gohhfpjfc.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gkewgknxy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gljxirdwc.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gusqnmpzq.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gidwrknqk.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gwkggvklw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gwfzifbtq.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gzlaktehn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gqzzoinsh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gvsqzqqlw.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gdhqruwzf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjzilazvt.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gycoeqhde.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtoxiaaza.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gvnudsvuo.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gqwrmmzjl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gvqyrdcns.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gulguyvuv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gmimapaox.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gnedjhazb.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gdnidcfxy.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gydrcmzcj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/grmanxtyy.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/giwziuizz.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gbjlayzdz.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gjuaercjd.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gqrxehusy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gjhxetukx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gccnipqhd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gbcmveacb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/ggnjnadyb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/grencopwb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gptibxpmw.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gyzitazip.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gjndvjhvh.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/glvgbmviw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/glcqlaobm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gnossoxsa.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gypmzogsm.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gmpkvozxw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/geubsqyqm.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/guklssouv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gsujusyir.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/grsblditx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gimbwnhvb.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gtkripfmj.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gxkrdzrvp.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gekoioyrd.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gtwebvris.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/ggvuektyk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/girdpnfpq.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gtnowsesy.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gmetadnyg.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gqslqsuym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gerfnhaun.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gpxkxpfin.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gzecvbugj.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gidfkyjjj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gohconnel.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gingnnrfh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gswreizts.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gbmfttuwn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gfaxbroqz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/grcxmtnei.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/glsjvcthd.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gwxwqnkrn.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/glekadkjw.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gjewsvecg.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gnfhrwsua.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gnlvtiqkq.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gnccudqdt.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gcuxklquy.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gtrrvyqdx.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gmnurxwwq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gmwcexdqu.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/godzskvwn.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gsklfakap.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gdbmmkuqe.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gqguzrifh.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdzqwaytm.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gvhqmyezm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gyveekyde.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gdfdrvdxe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gxiewiqrn.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gecijmzhc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gxdxkbkcx.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gxvonxxjd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/goxalzaru.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gxskxtjzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gpxgxmkog.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gwuafzkhp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gkvodhsap.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/goysarjkx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/guvytknua.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gqngwdtnj.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gqpfydveg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/galxtbnyi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gigitpsvj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gxlttkivo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/ggbrpcbrv.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/guhqjtesi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gdohsjrec.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/ggelnldyt.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gpjkgigir.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/goljeqhse.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gbsbgrmki.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gjilkdehb.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gpmlpiymv.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gdjpqappq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gawymzpgc.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gpthawnty.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/grrieenoq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gyvnkrbjy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gejitqtzh.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gybgyfjnp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/ggeznvocb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gqcnamfyq.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gpwrcmomu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gfipxrwst.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gciqopxvz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gyiqmmlou.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/ghcluiaor.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gftcbbjqm.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gvizicuav.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gvusutgbv.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gkidtotex.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gqhcpycmh.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gotssvwfc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gvsxwjzmb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gwruuulyd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gnixmiduy.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gpksabtxg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gedqpvpqk.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gybiggfya.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gragjbaxk.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gomazibdx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gzyjyfjjj.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gigjivhht.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gloxjhkpr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/ghbypgnko.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gojwuoyfk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxduiuqoz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gpcitgwtt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkvziepqq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gxdodscwn.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gdbhqdxpe.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gsnjikmiq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/ghmlqtbfr.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/glvfngznz.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gmmaoxuou.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gnjgvseva.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gppclktir.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gojqtftcp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gqalsgxng.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gpviigfly.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gareoogwr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/getmzhwqr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gbklbjmhf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/ghcaxtooa.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gfdosacqa.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gdbttdjos.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gqbunrsjd.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gdhijvotg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gehpkxnbm.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gacfmcufw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/godfevoci.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gcgosgmco.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gnsplkupk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gxlzkship.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/goqeernzj.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gxxcwpgzz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gmjwktzsz.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gxfzgpuvm.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gzfupqtns.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glgglpdhv.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gwydznzga.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/ghzmogqzr.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gvakpqvea.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glxujnedc.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/ggvsqnppw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gmsdwqjwb.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/ghvworuju.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gddykbidg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/ggdsdvyip.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gvkloeupa.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/grfdsgkuz.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gdpgxfhwl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/ggwtsgfpq.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gflxnbman.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gkvnxmsxk.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/grelaxidf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gbjiassbl.sHtML


<!-- 参考信息 -->