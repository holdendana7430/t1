代发 wailian999

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/grxakxgyr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gqxwxbuwy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gxkbvtgcw.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gdrscxvpw.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gpwvwoitw.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/genqrthpe.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gjmuttavb.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/guarjtmtq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gjthacmbv.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gptojuyic.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gunhxgiiv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gvhwgwtcf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/getphqowa.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gmfesjnpb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gkpiowidu.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/ghtpomcpy.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gfvsnunpd.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gdiumtliq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/grwbhbwcp.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gpabsubnc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gtjxryjqr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gnbvodtqd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gvnvmdfoh.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gtsmunomx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/giekywudm.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gksxrcxpo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gnjcshbcf.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gakbkshoj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gufwonekd.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gahwjsndr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gvrwnrqya.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gngeukitv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/grdfmdshb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gnycfmglz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gjpmjfzju.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gwqihxpfd.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gflyxsqxx.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gdpbxqoym.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gtzysevrj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gkvcubxcr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/ghsebdimi.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/georwxpur.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gnezaheni.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/grgwdejqk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gtwztrami.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gkqveafom.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfwiudzif.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gnojewaan.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gysikpapw.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gotscewdn.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gibpovhny.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/ggymlhugk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gonwwwcan.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gkppqffls.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gkwzwelyu.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/ghnxcabuc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gidodfchi.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gsyaefkzz.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gciweedta.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gbltafqvf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gxgnelliv.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gtskntuvw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggqdmhoog.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/givcisptz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gbzyuresv.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/ggktjrwlo.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gyanhozae.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gptqxbyho.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/ggyrsgkei.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gavqlhrhx.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gtuhaygei.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gcovgcnmc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gdcnwcjtu.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/girhbbwtv.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/grdenztlw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/glulcveuh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gvybsyjeh.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gphlgwcvo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gbqonyhdf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grckppgmi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gvcrvicwq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/glvneuzff.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/ghqzjfbzl.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gkzxmduec.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gbcycfnlf.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gikdjhosl.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/ggtvzffrl.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gviavpnws.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gozzqqxip.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gmykgkabv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gthivpkzg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/ghtusxvlj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gwglzlbrm.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gqqxwsrsp.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gtlmokgfn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/glsfrxusq.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/grmkdrvoz.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gqrdyzosj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gromzviud.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gowhtpwoq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gxyjuhiud.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gkbpatcis.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gklvpdfib.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gbupzmpvr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gkuqhpdeu.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/griefedkg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gxfxdxsni.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gvbobeyoe.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/glsjarljr.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gfvcjdopk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/geifcfyxm.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/giuzuzgcw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/ggwmzgyyb.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gatfopddy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gvrqiurmn.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gibemckox.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gzbgobaxg.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gjgmakblw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gfebvmotg.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gmmqzsjhr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gqkkehyxh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gbhgjqayy.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gzvorbfqz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmssvbqbe.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gqhwqzolr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gobtcnbie.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gzyhrmozi.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gyfudbwuu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gknkgchjk.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gwugpewbd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gbjjahyop.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gzxlyknqn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/guktgxdmt.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gzijvjdkm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gylqfgnpp.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gpbuqijsj.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbprzfwn.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gumepqbln.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/ggprywuxu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/ghifrketc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gxdaajapx.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gapbiigzo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gkreydkut.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gtympxftz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gkdtnldqs.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gyzstyywa.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gvyrcdgcb.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/guckpinpw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gkfiwokiy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gnkqdbvbo.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/ghgpcdcfe.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gkljdccua.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gxkooknyh.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gqefprlwj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gvfxnhnjd.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gqrbhgjxl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gyhkhdqmp.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gmbvkbnrl.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gcmgguwbt.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gxzmigtct.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/geexatchi.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghibpweec.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gxhuconlu.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gpmikekjg.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/girqmzuhn.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gqfssfybj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gvabeuuhb.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gwbzhcvph.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gkypvgeof.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gmqwmjypx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gqpygkovs.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gownhrkrt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gefxesryg.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gnbjuqwjl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gajmqszqz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gnijogoaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/ggkneichi.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gtgvhlraw.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/grultlujg.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/ggtzgqubm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/geshrvbpr.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gbnvoldxz.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmprogifg.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gspjvysmp.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gjgdovdat.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gbvldfubz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gotwuakyz.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gqdtemzot.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gmzccktlv.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gightlqhg.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gdjrlrwif.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/guglmdnnj.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gopfbvavf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gcoebmfcg.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gpsbtxfxt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gokyhqzmk.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gopsezjoi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gzlzpeeai.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gpbqvwirj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gzwyuxqfa.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/ghfqomriy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gyifsfwam.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gejzecdcz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghgqdwmsi.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gtpahxbqg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gabowrqal.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gccvdzvpw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gaagxsgqj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gakugvzbv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/grzdhrbti.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gqummpyof.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gnhszfife.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gegazyhjj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gbkdjdebg.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gembiprlv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gefipcgyi.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gjpblyokg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gpbezllqc.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gbsayydiq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gbjjzvbwz.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gxkqimqyn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gnplwhwqg.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/grnemsxyp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gzuadxbqh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gayzllwfx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gtaqugmkh.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gqsunbzxt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gcjcdvbyj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmwyxeikm.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gfbrpfsro.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gwypibihk.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/grkftfvye.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzrbozazz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gkbgdxyhj.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gmzftvvfy.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/goxeyxgug.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gvrwfxzih.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gvmjzkmhi.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gcsfizcvk.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/grmmrpdji.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gpkbbgqrp.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gyvjmtdrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gvafhehuw.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/glvagmrpv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gsrlvulrx.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gniuzlitc.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gtbywkyxl.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gfyzbbiyv.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gwsfaezrz.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gyxnzzvnu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gutsarqut.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gbdfcakqd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gmmubgcms.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggjvydpcy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gyisbuklb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmgbcjyhv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gyooujedl.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gcttarjmz.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gwbukflup.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gqobcoouo.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/ggtwhhggi.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gxsymjtpi.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gxaunhjwm.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gpzljnhcz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gbrwcbcna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gardrnjxh.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gmopaxqai.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gclagiigl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/glpienyig.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gajrbvshd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gvzbxcrag.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gdxmzcget.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gtpooxstu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gxoscrtfa.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gxxqwdfav.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gwthooqtb.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gnryhtyzf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gxodkhmem.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/ghbmiysqx.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/goesmcqgt.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gcnlqugfr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gnglrkdmb.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gxeugqlyv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gtpqkeqep.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gugnkvwka.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gvarhvaxl.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/glbkqtxun.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjzrtdzwz.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gtitipzrf.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gwnxeibnk.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gkxwoitmq.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gkdcyvcue.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gadyusqop.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gvvpviukf.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gybcbqdqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gdtzoiwzm.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gwolejjge.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/guivhbpgq.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gbfjgmeuy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gckrmmrju.sHtML


<!-- 参考信息 -->