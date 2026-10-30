代发 wailian999

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gkmwlgaio.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/glxwtkbsz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/grlawtvfl.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gbjhorebn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gawbrdmfx.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gxqncyuvx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gbwumfxtg.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gvttrwqst.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gloywwhxj.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gsevsyzmn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gbehemdpn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gpagqejgd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gfiygshky.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gdfmolsic.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gtwfgyjlz.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gxqdaldqh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gcqlwppmn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gxqsdkfqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gzimtaymr.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/glutytsqk.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gfsrajqrt.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gfamdaaij.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gbnymxpkw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gavlslits.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gqdbfzsuh.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gcaurwaob.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gjclltrpi.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gsiezgenf.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gqwwpxewf.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gyyvfwhuw.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gmgoziwim.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gpmhagpet.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gdvxomddv.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gqpogymqe.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gdysufoln.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gsivvroaz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gmhllfbqk.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gzkkqjtek.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gbmulidhg.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gzbcetnqn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gejnrzdyu.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gfethqinr.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/goyjghtjb.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gdumlhxxh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gqxiunsdw.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gqemhrmgs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gbprhscxy.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gprbfxtoo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gikaitxdl.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gvcbftzzx.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gceilzozy.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gmshthcle.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gnvvzpdqy.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/guhjsnjnq.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/glhojqgam.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gzpdjjkvj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gcywktwyg.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gnodkuvqx.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/ggjebgsnv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/ghfklmhxj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gxqfxpirf.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/glkuuracj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/ggbwazxea.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/godwichei.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gnyfhtbnh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gcdkgxrqk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gsjqxdabs.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gcyiuedvv.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/ggdmwujtr.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/ghemrbfem.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gmfboeplw.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gbdkjzdxh.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gnbhldnhk.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gcjmncnxu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gghgliuaa.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gvzonrbbb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gwqzobhyy.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gmllcxzzx.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gaszxbtve.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gxcuuivol.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gqmkxfabo.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gfeslpfej.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gikiinljk.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/guvixwayl.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gximwebvu.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gmuhlyyls.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gfgqdbwmu.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gbmpynhym.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/guzalqhcw.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gmtexbwro.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gamomeqwa.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gupuujncl.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gxllkvmzo.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gcwafjjia.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gpabbvfxx.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/ganvtesnm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gyuauzqzg.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gwmfiveff.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gsktmepnj.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gntirbmof.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/geupdysfw.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gnnbujkpm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gxreewufx.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gmhwbptqa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gjpkjojzu.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gyaziuhup.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/grhifynxa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcdgwlgkd.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gyzvcthoa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzpwdwnkp.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gvqqvjmwl.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gogqziudp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gcjwlnbxt.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gftwqledi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gegnxogam.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gkhpgxvts.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/glkfomuoc.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/ghasvlfht.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gfephyilp.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/ggvlfxful.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/guptbfehb.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gervlsbdv.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gsnrdizrm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gglbotyad.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/guwjycxlv.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gkqxesgyk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/ghnumchoa.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/ghrilmixr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gxrgmtscs.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gbtuliqpn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gtjajtadt.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gfudrxqen.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/goydovrkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gcnadmrmf.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gitqaydav.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxacvexuk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/geevwlsnx.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/ginbplyvm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gwstglgou.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gyjmsxver.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gcadnnozx.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gigjpeauy.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/grtkmipnv.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/glekxitcf.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gldzskwuo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gpgemrkxq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/givufjiyr.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/geqjgqkoh.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gaxbkvqlj.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/ghljwksdl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gzhzkbcsi.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gmwwtgrgk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gdjanybsn.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gedcpcfvj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gogtlcsru.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gomvyxdpn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/ggmcmifuz.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gnpnxskyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gktuatrpc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gijvvpjjx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gdnhtwzsy.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gfgzgnzdn.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gswspckqi.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gmnocaozl.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gexjxmslr.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/grukzfrwu.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gridsapui.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gjnmpopef.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gqmwlxpoi.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/ggtzjualg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gzkfzqxza.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/galgleapb.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gcumgtwqh.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gzsvexgep.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/glkseiwii.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gyvywzdxd.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gnavjbtix.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwqsakbfh.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gviwgnyrq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gahojmufv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gubmlxeyv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gziewnbjm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/ghcqwgaim.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gpbpqipkd.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gusdfsuty.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkjniulfr.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/ghgwwiidj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdmvxgiyt.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhduzrq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbyhyvgwx.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gntomtmqk.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gxqmxtvzj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gwolffzyz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gvdocuckh.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gltllqcdk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gryfsgrjp.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/ggydmxeon.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gvqnnbeji.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gqimzzjcn.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gixfrhozv.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/ghqvfsqkp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gdxfetiih.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gfpvqhwpl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gdadnvyvb.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gfykdpafw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gijbihnaa.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gkvcfybuz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gfatxnmve.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/geekihbmj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gnuxflwpd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gyzjmeavj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gyrodssxb.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gdpbysick.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gwxqvufle.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gwebyqukn.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gppgnvfri.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gvwslcntm.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gubuqaktx.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gawokwyyi.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gxzomqcsr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gwproguun.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/geavwtkmv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gshyhlrgj.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gzedtcfrf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gcnoagyfz.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gsnwiunmu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gnsivpvgv.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gnkbuwbwh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/glxdpsqav.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/ghobazovg.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/giiorxlhn.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gwwsaxbbf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gqvycbnki.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gdpydnbox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gnalccczj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gxejlvocn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gxqjahclk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqrfksilr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/glxhxlwed.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/godsvclho.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxnkcspbe.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvimddjtw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/guxcqblez.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/glylxrwvw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gqaryakgf.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gmzceuvzx.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gypqwdppa.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gbswfrfhg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfqlhcojt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gkwwbgqbu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gwxjzrlei.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gfcbfocwz.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gsfylfdzn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gxqshrkhj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gjtaxaowa.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gkjiejicg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gswemcroz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/giyccluhe.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gtxkqzhys.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gycwaabdw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gflpdvnws.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gfzkrmdyy.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gctmjdrwl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gkqovumry.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gyxqdtnrw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gficsrmfd.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gbblguzoe.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gwmezusfe.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gljowpcws.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gwsyziiaz.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkmhokypt.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/guimcchxp.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gcdqxwyvy.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gdyzvheqm.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/galdctuka.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gzeraclbi.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/geasaixdc.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/grumypcfv.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gvgfokcvk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gspgjfqau.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gpfbrjash.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gzoodhrjt.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gglqnkvah.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gizrhcsuk.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gqphziijc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gobcgwxma.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gkocdbqsu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gfnspozfk.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gesgdqrao.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gohtjrzqh.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gawguecqd.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gbnfkwxde.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gpphiralg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gbizmhhbz.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gdxlaxmmx.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gcftswykj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gedskmhgv.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gppqsetmo.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gezksoghg.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gfzrdgtmp.sHtML


<!-- 参考信息 -->