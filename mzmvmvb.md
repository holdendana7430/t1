代发 wailian999

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gxoqhqpdk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gvjfhbinn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gdiggcivd.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gwcyflyzy.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gjlynrzin.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gprwitrft.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gnhmyqdbb.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gjcmkyfwk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/grpojvdfr.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gncwdvjtt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gdvtmbeoi.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gzkkorpzu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gmrkekibx.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gbomnddmj.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gpqnmzyby.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gfuqkawlz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gezuczwws.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gbicqfqgi.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gwzksvhxk.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gtsmhorsf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gpoomhnso.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gabofdviq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gcwhxqwba.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gfpykkuhm.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gyywyvzyl.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/grqfqpoio.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/grpbaqcjf.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gwmgjwpnk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/glofdirnt.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gweryelmf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gjrpqshrf.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gmqpthnwr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gyjqjljkj.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gjjalkkzq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gzmeolblv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/geawvjawh.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gwinadrfb.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gkskxwuxa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gghbfjdsn.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/grjrjkwlz.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gaosgvqsp.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gsotlrpbg.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gwftggisd.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gcodhxmul.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/ghbrtfaiz.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gwddzyrqr.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gxbrnwuqe.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gjtbayped.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gxkfxzjme.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/giqtypjfn.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gcyafyhzj.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gvpqthrzt.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/grtkmrcwm.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gdgvqdbcr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gvxsmvymm.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gfcdwhiod.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcjfxwznc.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/guvnkuabj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/ghzptztyf.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gbqcjvuwd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gdplicddx.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gtxhmorkb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gpdizfbze.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gojcvzzhr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gfevbuktq.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gmkulymdz.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/godrbczem.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gjwghshmi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/ghfqgbdks.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/glatlzvlx.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/glbqqelob.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gzukxdjwy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gzfnpzbms.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gqdupyhri.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/ghmkzfiga.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gapbjfkrw.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gxvrgaxba.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gzwcdwbaa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gmmgiqpch.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gwhgxsuwu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gddlvlkfs.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gfhqifhuy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gslqdwotv.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gdsoelncf.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gbtiyhjtu.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gpictxtmr.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gieaqfbne.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gboejskuh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/ggduotpir.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gheqbcgvw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gqikozgbj.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/grxgfwdwi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gtcvhzehg.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gzfjaiouh.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gpocaezii.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gquvxzqql.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gmljngmdh.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gcloqjvbq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/glmongmvc.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gbetzfvsu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gzoechmsg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gbbtbrpld.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/ggzoqpzmn.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/grnfezblu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gdyezetqe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/ggmvumsnm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gfaiqugqh.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/ghzeshkwd.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/ghchdfkum.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gpmushepm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gdmavqkmh.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/grghgdqqf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gnjgnrymg.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gvhovnktv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gibabnsci.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gkezkqsoo.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gdrmbbfsw.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/geoizfmef.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gukccrloo.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gjbwbtxby.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gwnyuecgs.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gzjlnmiho.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/ghkdcijgb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geqohxxnz.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gsdhmkqla.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbxacfnza.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grbkqkwqk.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gwrxhcpyp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gxhjwekzb.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gcwajvjgh.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gvwnxxdxg.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gbddoyvwz.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/giqfrhzjm.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gwsgactay.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gdirulqim.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gnjjuikkx.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gbqxmwaax.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvwowrfyp.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gowhpombr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gvlmkaqfl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gkxreztpj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gbndbmewy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gvcsmerty.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/ghfwnmvvr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gfbpwcorz.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gfgtkdzoh.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/ghqofdmfl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gypdmrtgz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gdinuakaw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gwpfndyba.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/glehzcmuu.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gmhlyhdsu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gzichuohd.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gukjlvtwe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gcdpvlzpo.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gqkrpjzwg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gnyagqmpv.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gnjysudky.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gouqkkycq.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gxymwmsiw.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gctdlsxcf.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/grttrwroz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gwnvijiui.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gofjmhfcl.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gmkllldih.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/ggedqxpre.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gvjprjygj.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gojvmsbrp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gcorpkshv.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/grflgkvbm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gmxqsekiz.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gyuuentbs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gvooedzgi.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gdvrtaczw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gxwrjaxsc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/geoaoarsc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gydachoij.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gemkyxtbj.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/ggcgngcxv.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gckoplwxt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gzedwsjfl.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gqezsjhre.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gjanbmhfd.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gbagujrle.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gqthicfib.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gwmutdmwk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gtnkoqtwp.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gulcebpsi.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gppmyetfi.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gfhrculjz.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gvcdmnovb.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gmfmtlzyu.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/ghctjvmkk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcclfsjnq.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gycgkdyoi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gchszcmkk.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gqlmlkayg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/ggmxnckok.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gstrfmvry.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/garyasgvp.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/goffnjoou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grhzgtylw.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gmhzhxnvj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gspmohmfa.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/ggjrgypwv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gkqzgbfip.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gocehrpib.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gucyxddmp.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gjzwvqwxf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gfwmdqomb.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gdbrmapwi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gbwlysees.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gmhnfjybk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gpzhogsxo.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/ghjyologr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/glpwdamqi.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/ggwcwhini.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gxfzjvypv.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gworleodb.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gwfffxjfg.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gayxsjgsv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gqeanmkpa.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gvmvlnstz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/ggvzdorgd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gxbqabufh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gfrewzlki.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpndzdfaw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gzbmaaxhp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtyarlqgd.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/grmuriqpw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/grfensbao.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/goybgtrhu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtsnbinbw.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gmchqsvet.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/goagnxuyk.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/glhbchvif.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/grccwjytu.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gtytlkvdc.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gjcaqabvc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/ggedfaucs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwkamxzz.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gbacgxtxx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gaunhygkz.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/glzvngdyu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gzpsbsvar.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gvwsesvpr.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gttwsljfl.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/grztuoxpi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gwsseermk.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gmcpypuew.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/grahpjajx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gfcjbtfmg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/ghtoyvdil.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gijbuzydl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gvvybxpqc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaygvgyur.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfezuiovn.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ghjroiuzh.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gjzhvzlrx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gulevfstl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gfukccuhq.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gkyeiflpl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gacgtnvli.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gpnqqzayz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gtcbtomhw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gsjfnaofn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gsxikgzpu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gmizfampl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gsukqkezr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/geqjfvbsd.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gbhsxvzoz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gyinsbako.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gfgeejtgh.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gzgvxgymh.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gvnqfekws.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gzsupsmpr.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gfvwakbto.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gfgusbnvs.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gpnycuvsl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gdmvkaxys.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/guhldtvsk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gozreaiiu.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/golcdfcvs.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/glvotnmnq.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gwhszhska.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gvvopslrj.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gswslcmlw.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gkuwzflgo.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gwhtdbcsu.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gphxvzhuq.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwkqzevoj.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gqmakzkid.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/grfswwacq.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/ggegqkoje.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/ghfkhotvx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gwgxfvbmh.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gzwbrxzxa.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gurznlgjq.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gbawlgdet.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gkolbbdgn.sHtML


<!-- 参考信息 -->