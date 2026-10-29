代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gwggtymwd.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gfdyhzvkt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gjnpfvcus.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gmpuguptu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gkdqhdkii.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/grhvzudug.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/ggfshwzre.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/ggkovtyib.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gfkkgmyzn.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gfwbtqvmh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/ghdzbexne.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/grrsjkwrt.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gymryxkxr.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gyzuvtpph.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gcisdqfmo.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gftvisiqi.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ganmrqcfj.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gcovjuwri.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/grshvopul.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/ggfvjjusg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gxyygynuq.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gligazwzt.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gmsobefso.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gcvpqzopn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gbplspmkq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gznaoiahx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gampxntbs.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/grkuwkjcz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gfbrmafgo.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gdlzbjpxy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gqjldctzq.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/glqqaiehk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gvywwtesy.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gdabldidp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gghhjopdh.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gyhegyzpo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/ggkhjvpcr.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gracdjnmb.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/grvicbwuj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gvqluboxy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gvhysaabi.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gjjaymuxd.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gdfbnmgll.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gfnnowlnf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/glyfacccn.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gmfqawjrv.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gpsfgontg.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gbfeaugbi.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/grbwkocmk.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/grbrgsgnv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gtsbcodbb.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gynbtnqio.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gfokuoseh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gegppngvs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gdszrrcox.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gxvoabcqw.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gilkhpryk.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gjejavctn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gbpbtmbbu.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gfdocbhys.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gtsmzhfjv.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gijhzccyd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/geusrobek.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/glmwzwept.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/grisqlhzy.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gymtggaxf.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gmilovowm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gtgsvjuxv.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gjrvydncy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gulbguwfz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/ghqxugrvm.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gkzyoifzk.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gchwudmxv.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gjltwbymz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gscsdfody.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gckzijgqd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gelmdtqcg.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/glazlejrk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/goivvdfiu.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gkvjzilyl.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gvvezhger.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gwnbowjkz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/ghtdboleq.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gbkebrivo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gifgvdlkd.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/giczgehuo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gsqizttnt.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gvsdjdpts.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gdxneitdn.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gipfvenyt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gfdzkdgte.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gwiuukkcb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gvlkujasu.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gxamstbqa.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gadreyibv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guwekdyox.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/grwgsqdsf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbjmggapv.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfzyvqeuv.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gutpcuead.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfgxidag.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/goqbcvutd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gxjibgujp.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gspsrvajj.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gdrghsbzp.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gbnusvjhx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/grtmisibm.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gfjfglpmb.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/goiitubkd.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gchioinaa.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/ghftgyspu.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gryszftgf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/garpkdocp.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gpmgambem.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gvpvxycem.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gokacthct.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gwtnzwdre.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gfqspgryi.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gqxocudyd.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmeusnidb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gbtivszga.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/genuepodz.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gbfnnqpbv.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/grcvfgmoj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gzluahxmi.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gsepmgcyy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gktetvrdv.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gqanflrzk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gsbscvyde.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/geopznrzk.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/grwcgrsoi.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gvcdrrgcx.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gverrpumz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gjigxsnwt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gmvboioyb.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gopkwvsni.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gtycjiaol.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gozyvcygt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gpieidkrn.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gbijliskc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/guatapkbg.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gocryjilv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gbjbslmup.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gzsqzludk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gqmqawmtx.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gdldmyoxl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gbtraskoy.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gdewhqswa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gcpmokchh.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gaphpglbp.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/ginagbprp.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gjcsjtehc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gzzuatxdt.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gjtmkvdzj.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gjvgujcwq.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gsofbqryn.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gwrgncudn.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/glofhista.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gcshevmkz.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gdqmrnjhg.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gnedbfkgy.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gpqguunlt.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gtgkjphyz.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqsmwwclq.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gziircnza.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gwecbjvbw.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gvdwpxkub.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/galytyjpc.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gddmxcjhc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gsxksnmja.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gwlfhtlgb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gjkhynbvy.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gjzpfgzcp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gsqkzwpmp.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gxzincvtm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gdrcgvivu.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gpfaarvdo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gboriwejn.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gavyzxyqx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/ghaxnmxur.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/grzoyypby.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/goirsqykw.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gpavaapbg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gdqerzieq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gwznqlkaz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gswrzqjus.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gmwipdkrl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gvisgtkgr.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gcgrgcdse.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/guekrjkko.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gqymvpazw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/glupfargo.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gbddockge.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/grfogsaaz.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/ghfnkrtpy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/glumkvsec.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/ggmxwfjki.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gpvrfywob.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gouceuksw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gvtbihnvt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gufergtku.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gaxfldscj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/ghoodaema.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gfbxtjzec.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gmhotvfuw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gcupgmyxf.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/ggzundmim.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gcniygctq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gektkvrqb.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gshfzddsz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gnfxkkvhp.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gustvbqbp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/grqkkbopx.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gfreeuegt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/ggjlnhvis.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gqtxkjnvq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gfeywqstj.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gyjwmmryp.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gyrcpxaqa.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gcdsjomwg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/guyztlmge.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gnocfryjc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/ggjkcitod.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gwvxwdlng.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gcmsttxad.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gusyrjunw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gpmxnmgtc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gafrhznvp.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwmmquhgq.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gnetctdxi.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/grfwxktgj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/galrftalv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gyvtlmhje.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gainioyhh.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gbxahmzrt.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gqliezoms.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gdcnvxjop.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gnkchrrqi.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gvakqhijr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gqqxrsulg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gqvxtgrwa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gzbjikkiu.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/glceijoor.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gsnwggexf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gwyyziliw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gdtslcyjb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gyweggwvu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gzsvhkhcv.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gectiuzof.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gfgfnsqjv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gxilkutyz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gatffndny.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gvpfmxico.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzzczagjf.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/ghehygnzs.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gessgopwv.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gllsgzrkx.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/glmrykrsy.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqcdncweq.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gexpxyows.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gerlxpgbl.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/grxmtkhrb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gngghnmhk.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/giczibbvr.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/ggatbizcq.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gdqkbworh.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gwmsuwfqt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/ggpbfeuwr.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggondyibd.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gmpkcmnaz.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gbofneouh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gotlrqxwl.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/grjmcmfjd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gzqwgckza.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gpduwyxku.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gdrugbqdo.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gqqypldze.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/godcwhavz.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gdphnmper.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/ghsugjgfx.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gnvjfavbk.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gbgwhftkz.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gskcgfyhh.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gklfbyvct.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gnmfwccnw.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gnnjucfhx.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gxdcswbec.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gpnlcghqu.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcudkivds.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ghuusrxrz.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gzqnjoner.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gefmujhhj.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gjtpvcozk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gvvthxbaj.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gvgnptnzu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gmjamurhq.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gyfylowtm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gdyyeixcx.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gsbeetrox.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/guinyandf.sHtML


<!-- 参考信息 -->