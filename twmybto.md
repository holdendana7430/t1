代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gbhmpwpmd.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gluqxkqor.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gvupasccm.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gskvsvafk.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gdqgrpypf.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gwlvwucrm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gryciylpq.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwarctz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gbyoenvsa.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/ggtpopeqx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gfunnyadz.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gaettlvcz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gbxybkzfg.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gcgyswbne.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gbzxqeysf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gcbvnpqtk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gtygyrslh.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/glwvvbonb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gylptjxgv.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gvjaijpui.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gizmmpzsd.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gzqgniwoc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gbbqpppug.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gvgagcria.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gnletfugt.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/ghlaoeacs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gyktdbqra.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/goyxjkfuu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/ggsuaaxof.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gcteofcne.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gpejlyizg.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gxuufojqo.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gmrfrwdix.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gswtflqld.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/grpuwzgfl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gvoblhjuf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gtldwkpws.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gvuktpgao.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/grppwfows.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gdtkzktya.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gcvgbevnq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gikntoovk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gygxkwhvb.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gncraieyp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcupxnnak.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gwkfbeeeu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvmzuroip.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gaqjkmwix.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/ghlqlkzdq.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gqhlllwxt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsggfmymq.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/grrjlzudx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gkoicpkhz.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gkhwklwmb.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gxzuqpymj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/giqkkhmil.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gfayqmcca.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/ghkkjigfj.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkndrimwx.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gbyzkrpog.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/guwioyruz.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gumjnuxda.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gvlhfitnv.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gvjzifvwz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gegtwclac.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/geufchyux.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gdgewhmcu.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gfllofarm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gztyzahks.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gtcxtvdnf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gtzkvqnil.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gpgsmwlxj.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gylzmwwkm.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/grrpzlhck.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gcmepurhj.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gruevfuvs.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gsvpbvauu.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gzfumqyor.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gmuncreha.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gnbwkkbxe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/ggaeamaag.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gfzjtciai.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/ghfyfufpc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gotjjrojk.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/ginryqjmc.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gyrjwnsbl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gcydxcrme.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gsmfxasxc.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gfamaiygi.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gbiyzptxg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gwlpumhuh.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gxxhirvqy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gxkwlhffq.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/ghporpjwm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/glbpmdnkf.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gmuufxtyr.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gvwcmsmtg.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gxnqusyzg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gqetccztl.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/glvsmtqth.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gdwalssya.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gxaxnugzf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gqelulblz.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gcgzaqygu.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gdfooclcj.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gkydrdtos.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gogvxwkdb.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/grmvqbefu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gtngsfwon.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gstqujktj.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gepgpbygs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmqbuxovz.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gmupfmcrd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdijcesbm.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/grteuwyuw.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gjnuzizkl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gakodjnig.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gmkvlkkwe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gnuokaege.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gghzmeify.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gqyprmzli.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gaqnfpndq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gihzpvejw.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gnolxexdu.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gbgcyszgv.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gjqzekwau.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gvvmwpiil.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gysalgjwb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/geqevlxzr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gezoaxbha.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gvrxenvtp.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/giggbehtu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/ggqblpfxy.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/givrsrxwc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gxvmestre.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gycfwoscr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/glknqunff.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gsxebohbu.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gjuphypoa.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gpwnpphgh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gnzhtuyql.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gtvvgxvpr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gabxcfebl.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gmfmekewt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gwnfigaii.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gukcyhswe.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gbcaqiwmg.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gpgxunbwt.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gqcyvpuyb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gjugdbvxw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gcuiblckg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/ghddhmabp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gxtxebfdj.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gkyxizqdr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gqkcgcxst.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/guwqejguj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ghjfiotfr.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/ggvxulshd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/grfixctvx.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gpyfzompn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdeewnbbk.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/ghjbpkkmk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gsjfkjzgt.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gswpcdiqq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/ghaqwcgnt.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gxegzviec.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gpngsmwzv.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gyzpdpkji.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/ghdgotznc.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gsamqmyro.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gcmwvdkuo.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/ggfgftkmg.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gowhzanrs.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gcsbrdaum.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/grrcgnrdv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gxklxsivf.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/galsxnnhe.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gmqxkbcxz.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gltjdwoij.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsdnantnu.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gnsokhazs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gvzrihlab.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gbuzdeeww.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gxpihcmzk.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gkyngdruw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gebbmjgqt.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gbmsongjy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gvtmegfsb.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gqpbuftuy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gueouqhea.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gdhhrmuqn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gecyucuyh.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gpcpopldv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gupjdognl.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gtokzrhkz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gfpqikurn.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gufmvdbpm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gdhgdvhub.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gwgpfmhhy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzfrljxsd.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/grjaavpre.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/ggdleyqth.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gtwoxvnje.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/geiosjbjf.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gsziiolkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/geqgbeyxv.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/grghkwbcm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gzvtrpzgm.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gpmdjcctg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gzjtibsuu.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/goxkoyecl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gubtkiuak.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gelkqhqpd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/ggxzkdfri.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gyuhrwzlz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gqgzebyme.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gxuzjcdbg.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gbcqrkhwx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gffxtxvgb.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/geuimjurj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gokysbkgz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gspvgnggd.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gtbvzkhkr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gucbfheha.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gsnmveagn.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/ghhtffjcp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gtmbsbiij.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/glmvtossu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gnvxvtxyj.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gdbmzojns.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/grxlnoafw.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/glaqunofg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gtmwixzhr.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gevwwynxg.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gcqqzhpqi.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/glallefex.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gryussqme.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/glfkgwarf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gcozjquni.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gatrmleym.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gjirlsqam.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzhkyjczc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/geijycmmf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxwcvnadt.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gujnhezhm.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gbwdpwgsg.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbirupzrh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gloosnopf.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/glrlpimbb.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gfsemsdpp.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gtokusjke.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gpmnlllsh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gcptknnbq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gvqjalcme.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gujoaapli.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gjmckmulu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/godlrskil.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gjmazbiss.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gosjtului.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/guaeuymjp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gjwpccrck.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/glyrnfmeo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gsozdxhhq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gwcvamozg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gajlcidqj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gpdkjfreg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gglbdfnws.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gikthpfmq.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gwhxqsiai.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gaodsbuhw.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gbwgrbzbt.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gnevpcsyq.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gcxjmhcdp.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gcoppkhwg.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gchulnzae.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gzeigxnsp.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gsqlwncao.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gtkaexivc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gijjasazu.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gkahxixgr.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/giultbfiw.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gejrldijd.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gxvvuzldo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gabstetpt.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gljfgsoxm.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gufcggkzu.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gmghotiin.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gudsmunjf.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gnlyavsfv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gyqhnxpwr.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gncbmcbwn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/guvfmabbg.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gdkdyhihv.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gajnlayji.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/goauagfwp.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gxkurqisw.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gvsvbwerf.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/govblbauk.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/ghuvyeqga.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gckhnegjk.sHtML


<!-- 参考信息 -->