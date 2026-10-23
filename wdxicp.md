代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3lwtggupj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mlqfjqua.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3emhdgewy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tlamfpos.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nmktecfu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dczrsvic.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3apikxcjs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qohvibmj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3azrofzyq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3suzrxgxj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3esphjidf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hrckjdso.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3abnryqkv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qfborivf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ubzburzu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wuwpbbzh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3sqjoxzzr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3tzxkrppp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zdegcaqs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3awguhhfn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3euugrbzt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tdmxhehn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ozqlwdhw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3txepeuiw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pbfbdkln.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dyzjijlr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3admfstaz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxvxtqcv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jwcuzrwc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3iyvbfgdf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nytrjbhq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ibrtceed.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xotfomyo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3netfzfyc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3rzxkgkhe.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bcnynhbg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fffpxkaa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bezvdogz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fpkjxrod.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ndxtpyeh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3gimqyami.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zbotohba.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gfgftysu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jfidjasb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dxulvagp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3makbsuls.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fkijbyru.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ziiqfboc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kkiorjme.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvzunlqw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3msvctbgw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3eoanovkr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rbeprcdz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ujcfcump.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3esxdupix.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pccszgmp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3paexhksn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xftbsmgl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jsgehxee.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rxvpdubl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ymolwrbv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hnybftfq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tkaatvdi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xvmwmbem.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ldhtgmmg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3eadsvyoe.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fdrjmaki.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dgtslzkg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3hztfygel.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tcwsytqx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gviaquah.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wtxyykxg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3higttjvk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vghypozy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wvphngzg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hpoqfzrx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xtqpntvs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fmutypyg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xmfbppfz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yrxphawl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yenkxvyt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vpcjlxem.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3icnooirx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dwqwdzcs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3spaixolr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3sakbeiqq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pznjogaf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3duvnddpi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3csfwcqjp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3itnibzar.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cwlkkklr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ijbcikoz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ctiyozhl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3urqofvxj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3oscmzoxm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xluuowjy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hjsfbfkr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3bgcuhjnx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jsziyxiy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oxtigfxn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mgiurxix.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3brzoimks.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3szqwsvqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqbgsvvi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mmjprlhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukxxmnzu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wyuqdssu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ijccqeqf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaomdhjv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3joixpnne.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zrjbyehz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kmpumhxw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gopbdalq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3husfogdt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3owgmfhex.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dcuyruwx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvsqdnm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3isymlatd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3rhyxyelz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tanhxapw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3napoizpl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ovdgalcw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3wiluffui.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3wljflwtm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nmeldqhm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3edrblonx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3icvdrsds.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqydmiaf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qrphlesv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3guubiwdv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ozyzxvdx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwftvukc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nlwkzitm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3osomygwg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dpephqus.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jxzjehvf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jqgaamns.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gawpiede.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hoagrwhn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3uvwnlhxd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3iylkyshk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hdxutwua.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cvajbwsj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yhyzdsfy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xerilvos.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3stdhyrmv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3coppkqbc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rfoqzbbp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3daweuhfl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gdafnwfz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tftqurrl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nzpqihof.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wdzrtemx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zgweqepu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vrsfozrh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hvbaqxug.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ofhfxwvg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3avmlpqua.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ceixkuur.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3imcibtzl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vgsvfceb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ibfqplfi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uzpkcafq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3klwhuwkr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zjfamiqv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mgqrywhd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gvgozurx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vgterszk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uiqfsipp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hgdbaoyl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3eoilmlnf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zooolqav.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zfriukxz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilrrmhof.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3krzhjwnd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fxbszuiq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ysflrawt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ahylguew.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vqvlztam.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttuclxcd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3paggrzqd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3byrmvqrs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ccjaefjo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lulizzuf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xzedormr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dpudktoo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3yfaxkxbl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3knkinreb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3sqijedpe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3kmphxtze.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uhmknxsi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3imgkonhq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xikqqgpl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jxpowfld.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3olhivytf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ordydzsj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ppsdvwyf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iejoixid.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rzjoulff.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbuondnb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ksqhzpbg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fiwxgxnt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hupzmxua.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dakplmyf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yrqxjpsl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wtwmfppz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yusxcaoq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xraeqinv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mttqkbcc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qfjdfswl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ikmyycge.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vggfkhdr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dlvmekcj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nwmisqsh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nmkerciu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rrngiakm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3icblftop.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zusvwfxq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jsqszfqt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ewamvqws.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qmmjmice.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kcxpsgjy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jvxehfxe.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3axnnatgr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3eazaqors.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3oqqdovmp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zhsjjfqu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vauhltuy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3kjmvwjcr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3sgccvods.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mddyipxe.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3luptvjxb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3klkxmhso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oznlwpmz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ijcenifb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qezdzubd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hcudsgtv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3trhkygjz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ulgclzsp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3syvmoikl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ahbwpcps.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bxiojwed.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vkcywzlz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ssiamnnw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qxeznyoh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vakdhgdc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3twkttuuf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3whuqxvji.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fsfjchkc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ntiyeuwp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3twjmijei.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3adlzbvdq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bjkxtiqm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3atophazy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tigjoeux.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kdwulpkd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hsuphtri.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hrqqouql.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3nhweizoc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xeyhwaoy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nmadyybd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qgljuyae.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gcnndfdc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tpjxgavg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uetjdxxw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lepkqkgh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tdljkmjg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3adyjsrpa.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3tierjehg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ugekldso.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3puazhnjn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fjaaekvp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sfeojcas.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3auzymgvj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3sksqnmvl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ntvqknnd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jgvrxhjj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3olgowtjq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gapwlqao.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lmqlotex.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vsgvciqc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ftsbpdha.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3djluzafb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3neorjbuu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jjnsxpbb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gzbpkcch.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lpwkvotb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ueqmrujs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dyirwqvp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywbmlqig.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3potixxlj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3llagmdbk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gkynpjxy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zoltajzc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ztbjlhgn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ummcumdu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3azgbfdrn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dqscbabo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zypltqvo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3inaqsgnl.html


<!-- 参考信息 -->