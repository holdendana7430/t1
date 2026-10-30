代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghexslsrl.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gaammuydy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grumggtxw.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdxtxlxm.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwymnycf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxpsknx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gejjumbgr.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gegnxdazd.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbdazcfja.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gaiosrcen.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gevmzwptu.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmmmuqopg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcjllbrv.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmwwkqtm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gahkzqiak.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvbhqdvu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcjpnbkaa.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsapppsvi.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpfqhpnp.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwkgnnvs.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gcmkytyda.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gdxnyfzil.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gftrqtxww.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxiyfjpwv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqnfwjqj.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvfuobrf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoeaggnt.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnjqwayj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkxtknfl.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhmafgfx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgzcssue.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezmptwot.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpubaeagc.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxmzjwkl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gamuxzonz.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gdpxhvokt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqvhewkm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gggvihpin.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gbcswxmgc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwqlunby.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gszyomahk.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gettqinjw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcneppeir.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gqqqfqezv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdouaidi.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gibwarebt.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/grggmlaje.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gukxberux.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnavklutd.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gxhtltlcz.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhyyzddm.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxwftdju.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxcpuvvr.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gghyuhnub.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gywxbhcot.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzakavzo.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefcwrzhb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gwjdeaxgb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjeoccel.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzujpekcy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyosxlstk.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gldvsaznr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gatagsvau.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmpyanuud.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gzdtflgcc.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gwldzpkqb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnubhzuzr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmswrbrla.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/ganlipnih.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxsdvkob.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmrhyddl.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gnmemuswv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/geaflkbfy.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyfdkqueu.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqzqesfgy.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/galvxpdmr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gkkwoghnd.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysiahzsi.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gjleklyfz.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gjfosftdt.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/ggjhiidjp.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbkpyvgb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqwkukic.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnjxbehp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gritzxfib.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gonkkamnn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gwtolahql.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjxuifno.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/glbiqcraq.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbbtvpucj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gondugdnj.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvgybhwy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/glisvbrem.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfvpblhq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gvfjpjxha.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/garlfqxkw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlxqspqq.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhaxizay.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gtmqtcogs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gyhyskkwe.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnhbsxox.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gybncxrnm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdoqshdae.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdindonb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoxbpwui.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gfrrmqbjt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gafsiqpso.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbjfifkn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjooxenf.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gkatoelkb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/giitisujj.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwvunirz.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/getazomqb.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gohgnhzpe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojtwvrxe.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcpygcfa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/ghjyzysss.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaynztum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/glmgcetud.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdcrkuss.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gjngqahqs.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gxypboubb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gscojglym.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/giznllcms.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxpsjwdf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdddwzvv.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllguxzeo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gklsiqwqx.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gknmklisq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfhefdcl.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzoadlty.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gggykmyuh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipsxadkd.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/ghbotafju.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/ggidkyozp.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gnqckrknv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gktxrxkpb.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/glsnlontg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfexwyvtr.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/geauevvgc.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmxuhdxl.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrmqefqq.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gmshfccqt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gzihmjqui.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guedudppe.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gesyirbng.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlpoqtgh.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyytdhdc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwhquqwt.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gfjmeclwi.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gcvaiatwz.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzxvatxf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcddcdvet.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmviznecp.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ganssmlyl.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfztexis.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gecxqodur.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gidlyuqqc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsarosmye.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gemcpqmui.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gapcewlnd.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpbirhmb.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/geunsxzni.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/grzxvgjfp.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzoubdahy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbkiqofq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gacqvuwwf.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gtaeeotne.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gvyrjadol.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfjxopkcu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvruybvhe.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gzqggwhvj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaeeyqmz.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gvkzlyuch.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gigmbtywk.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkgpneii.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/ghynexkgw.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gmlemmftu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfbsaaeh.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/giqtxizcv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctvwqvut.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfwhxqnl.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/ghmnisvqr.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gsohitglf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gipqfrquh.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqmovqvng.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybmkonny.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gupnxnrbd.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gcwkzanrj.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gydlrmmlx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gxqghtzqj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcrgpwfk.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gqotofewa.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpxytzel.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcsmflqb.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvewpnwuu.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaowxkmo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gglawpudw.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/geicirxxh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnumlodfn.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gbbdiqlha.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbxqklxbt.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gyrdwhxam.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gglxilfjf.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/geomgedtl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gslittvgh.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsinowrs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmjcekpc.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gijebwmir.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghizrvqgo.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmdeldwxo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gywethmpw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngybxbgp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gjlopebbe.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gintryult.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjbkaksp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkdbqwnf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggewhkvka.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/geudlyywd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gznfepvtm.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/grqrtqdns.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gyctslwiz.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgnginky.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmdfyouu.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gbhdsjsfk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgcictdu.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gxvjqykhi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdbtijskz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjrkgltl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdxjxdyb.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gflsgcwcc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/ghobwtnix.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqsigsfb.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkujvigns.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gxhxjkaqo.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gerlugmbt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjpeegseh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guigmdnbj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkljdfskr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/guymjxxxc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhusqsls.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrjzoobd.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gpbyjvslg.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyiaqmqm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gbiismpfp.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gkocmbfgd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgenexut.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gzyczrnkc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnvfylthe.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyfglnec.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflwgdwlt.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gvfiwqjje.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgqfeccc.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gwtrwpqkx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdxhrkdr.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gyzrqiiuh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gggduvwdw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyelbipk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoafkxox.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzpnnmdm.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzouiiihp.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdoalfei.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqfihmch.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/grlnsgmrp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gcpgtdsao.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/ggdfkmehd.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gucfekzcq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvpduhqm.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtaviwpfg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gysemeave.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/glgctoqxi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwagborp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkrpzcst.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gpmnkkuoq.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gajtcnpfd.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/glojjpgba.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmfarljrd.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gijjugkzk.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/glaqtzkui.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfrqlkvy.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacfxjumc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gldgqlzcx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/glanztwpg.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdaujbuo.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/giyosfskc.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfopdoozy.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxltysyot.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwdkovfu.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbnsfzsg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniagktkx.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gatfejywk.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/grlqzudaw.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhainenr.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkbcoraa.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqmmgcib.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gpyjnjjpk.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gejwtzpal.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaafumvsb.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gntfrvnbh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtthzxxu.sHtML


<!-- 参考信息 -->