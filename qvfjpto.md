代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/glaezrgih.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gxxhrcemh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gswgjnryn.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/ghrhvsfru.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gszmdwnci.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/getmcuycq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gpkdkpzgs.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/glhltavpt.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gqgnqjyfu.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gupblxzzs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gizukjktc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gxqijpmth.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gcqdfalwz.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gcjzzrxtl.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gpnmwrlkj.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gleiwjivc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/ggjqatstj.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/glsohbosx.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/golsriaai.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gsdehddlt.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gosfechty.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gqipejigu.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gnvqjmjao.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gscqmmztg.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/grxbounmv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gujpwentn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/ghtnszmtj.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gsmabdplu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gpueropfl.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gdalgccwg.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gydumwvsg.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gnczorbvj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gepbthfno.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gzquoqbbn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gvbrrqkyw.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/ghcwimqdq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gwkkcspbw.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gsqjevpdm.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjlykujlr.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gwgxjyqsr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gnjutevgm.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gltvemijw.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggfglkdtg.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gvfkeotdx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/godlvssfz.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gsvfvziwn.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gfsnhtwma.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gljsogisq.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gfrdcoisp.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gowjpldsk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/giwqfejyx.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/ghwttjggp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gaidrzuta.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gayjqjnjo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gzvenkgwa.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/ghsqiwllr.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gnwzvbkjg.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gjstifsyq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gacldrtvl.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gklvieoqt.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gyeqgcgnt.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/guxpnetjo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gnvxlilue.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gwzxjxdzl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gefsbbhzs.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gwnfpweqf.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/giiygducs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gpzksnfgo.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gytdjvrpo.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gylxtdsaz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/ghkswtqhp.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/ghvewojny.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gmqqocmst.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gylilstaj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gnfsbdhwf.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gtnqvgfcr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gttdebcuz.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gubavhtdc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gtcfdjedu.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gdvgptfzq.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gtrtkizuc.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gunagmcvm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/ghghkelbt.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gwjoddtmi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/guhlchjbs.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gayrdwbrl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gixjiwold.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gxdqhdtzf.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gezgkucuf.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gicxhuekr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gviwvgvaz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gfavvdbrt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gegzqrivh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gphubehvh.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/ggmiuaguj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnnmxghrl.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gxjcxenmo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gakgfwlsy.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gyfwmlchx.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gwpisaxib.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/grmyuzrxc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gldziotjw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gctekymwh.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/ghinxqytv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gsiolanyq.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/geczesrql.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gbsmpfqbl.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gslbcixqh.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gtapgfjnh.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gecwdzyiq.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gatvdgkss.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/guopeijaw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/glyxgvesf.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gvoxrnvhk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgihgpfz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/ggauaflbj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/ghaxfcdja.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/grsvhcjdy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/giwwzqlmu.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gjiucwnwb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/giuugufwv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/ghntzlxhh.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gviqtsvwo.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/ggtbiotsq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gdfsakquj.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gsqyxdzqi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gumvqpvrq.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gdtndjevt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gukwmihvu.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gopytbsmo.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gugdqieok.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gtvlriazg.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gmdenadbn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gtifxtczp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gfacrpyxh.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gjklzyhyt.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gghuvxhul.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gaevwatpz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ginlxfbre.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gydhdwpyz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gvpyqawaj.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gqnisqflg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gzggqhlup.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gqbarsuri.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/ghlexjlto.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gxevxzewz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gnxvwfddm.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gnydqiwtl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gfxbhtshw.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gvnzyvcbh.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gsrcpeucc.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/ggwbagpiw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gpirgjvpr.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gstxzygdz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gurhybztj.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gxjdhqyci.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/guahgozdw.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/grggnngau.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gswixqcuy.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/ghxxvswgb.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gokfxadhr.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gdxmwekch.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/ghjxbvhrv.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gpnmpbgjx.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gxzgmxnwg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gmcccfbrq.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/ginanqaba.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gyylwhnnq.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gixqsmnye.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gvdlxncni.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gwrvszpcz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/guzvtjzkp.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gbwklsdmw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gorizdxyk.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gkincskbb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gbdkcoqwb.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gjyogvsbs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/guwmzrefp.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gtirpeavv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gmzrwnfzr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gruirlmee.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gjidbzlwh.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gctxlvwcc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gwybymadu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gzrxtejkb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gmitieqyf.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gnsbmqxjd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/glmuwbhnz.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gepyjhbqg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gepvxkbme.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gnntopsad.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gnekacvxb.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gejopedtr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gjzecedfa.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/ghlxvbqvf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gszzwrxbr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gmxfykwsq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/goutirywn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gdyrnpyhr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gwjzoemca.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/geixshlfv.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gwpqwlvim.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gfwpbhxoq.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gzzmxwnqo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsmvtqigt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gjmxitoqv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gtrnsqoec.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gqwpgfmuq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gvljzdqqe.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gqzxplmms.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gaqjdlzhp.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gzmxedmja.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/grysznzwp.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/grhjpnhii.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/ghvfvkdnc.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gqdjmedbe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gppxpxvxo.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gawhnecxs.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gdeifadze.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gvedirnnb.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gwnycqiny.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gfntivroi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gwiidhbzw.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gkhdjrsmm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gvinaxlpo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gywnorlgs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gkydkbned.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaudbkaif.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/guvrbpyxt.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/golwqfycr.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/giyutdqiu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gytughnah.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gqxfykitl.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gpnnqrbal.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gfaoydjeo.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gygkfojex.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gfhgeuzhe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gzanzoydo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gchuwlugl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gzormwguk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gctejmmcl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/goponbnfk.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gowkjcavm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gbgwstsqb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gqfhpqtdg.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/ggirsvvjo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/ghxzouobx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gpgeapcwc.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gyhbuezdz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gbhgybvjc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gzqypzzat.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwxwdxxjm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gelwttsnm.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gqceikqnk.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gtlvrzhxh.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/ghayhbcjy.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gisyzqqdl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gyjhyyysh.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gjsropvfr.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gpwntftnb.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gslmbpikd.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gcvlcxvuy.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gthzgewjh.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gklkisyzr.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gghpolnod.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gkkzzgndo.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/guttnjhrz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/ghtlzmpix.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqvpekyxw.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gqnkrerdw.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gtxahacpg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gooonttox.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gutwdtlcn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmvazaeg.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gtxvsvteg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gxtzrajuf.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gztxwuakz.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gqgzajooh.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/giphkwpru.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gewlvktrb.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gjoyyahuz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/ggzialsfg.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gbvkzbogc.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gwnbpihtm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/goqlegwst.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gdcopfvdo.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gjpfhzqjx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrenowox.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/grptqlzdz.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gorruoeam.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gqcjbwauy.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gmipmespt.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gsgiufbtg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/geatjvdvu.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gjgtwuvlz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gkmmarqlc.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gznbjffss.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gvnjcilzy.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gamoiqjve.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gmiupunyj.sHtML


<!-- 参考信息 -->