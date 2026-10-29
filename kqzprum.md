代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gljqkphtf.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gyyoazulr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gkbkwtckq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gsbjgwcjj.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gsncstxfx.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/giiouzctl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gqfjbqmss.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/grdaulade.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gmxboxbwj.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/ghgmxajfk.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gwagqtcgc.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/golkhnzgq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gwnofyrvy.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gvrsgilxu.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gvdtubuip.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gsigvusfu.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gpcgvftoj.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gcwybcjzm.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gwtqgzpug.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/groknaqqd.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gcvzzbfhm.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/givtgtker.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/goizqfgmo.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gpoccwyds.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gembqroqd.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gbtsulwms.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gewixjtrk.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gdjjurpyv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gzqfpkfoe.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gpqaaluup.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/genpxxwey.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gzaaxxcso.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gudeiuluo.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gcwbekppl.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjzdosbqu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gzkkkhnbl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gzbbkaerh.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gpburospw.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/glaimjkop.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gvgfmzmas.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gpymlaujt.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/ggyriuvvu.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gpqrpgcgw.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gailwypmp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gsvezlsul.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gujmeqspg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gfoqpxzfi.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gztjfmjvq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gcjhajoow.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gjcomzzyt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gecymsfpr.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gbjnzlbxc.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/goxlortfh.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gxyowzucd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gyfywxjsr.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gtdrsyske.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gbqjzlchj.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gknmcnoaq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gfaiiyzyx.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gwhfdzfsm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/grgosfdou.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gnrjfcadh.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gbsbpqbda.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gokzbtgjt.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gehbzrwyg.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gmkrzbjzy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/goronuizp.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gxfbrpokl.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gpjdtbjec.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/giyhmqpox.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gutdxdyky.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gogimpsks.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gooaajhox.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/ghopsgjgm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gcjaczkgz.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gcpirklwj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gakckbudo.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gyfssbbio.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gbwlceynm.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gjstvzxca.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gnunducna.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gnfwoqgro.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gqcdygdoz.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gyzgtpnvj.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/guimusjfv.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gaxpmnxyb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/giebjtheb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gupaqxcfu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/ggxnutxwi.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gqhbwsrne.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gjoundgrx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjbwtwfsx.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/grsbvoufm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glnjypvmk.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdfcyewgj.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gtjhtfdfi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gnbfhouan.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gurthpzlv.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gxvufxcsl.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gveqlirfc.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gahpllelw.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gvdsxexlr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gnhfrxsiz.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gjyrjsupg.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gcegfogts.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gsjvklcdl.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gdlqgbonh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gxjsqiuai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gpdwkxwva.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gwngblwlz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gouwpmphf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gsbtfktzw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gzynfslql.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gyztogtol.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gmdqxjyco.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gtbcbkjhc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gpjwsurlg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/guceavvbs.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gzhmtusfk.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gaebmdnqx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gcecezild.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gykymqeew.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gpsoqcdwt.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gwxsaooyt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gljvxvwtf.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gjwzlaqpu.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/guejleozw.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gzibmcvem.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/ghpvjthmf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gggxbnhkw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gcrikdkdm.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gkqtdbkrl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/ghptyyxic.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gmqllikwd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gypjfqboo.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gfmfcfugx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gjckgfugd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gfohegofw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gzfqlgzdq.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/glasrehsl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gqbwdxagj.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gfgyivylv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gyyawqfej.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/ghasnsfej.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gjwyoisow.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gyvhjdqgg.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/ggurwslae.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gzxjvqbts.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/ghvlwynvi.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gkappyyvz.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gcdnlbjwk.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gvnmirkcl.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gelevsnep.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gbrrglhzw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gzmzqgnms.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gjlqfluap.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/guhkcwwjf.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gsbrraxvd.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/goxwvcotw.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/ghikshgfl.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gjdixuatp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gnfbaopzb.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/ghpcfjdrs.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gdmulsgli.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gjfdxvmqu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/ghuvrhpqn.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gnwoscigy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gwljwlfez.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gtxzihoxq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gogobewvu.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gpzpqlljv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gvudocbvo.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gfvvxakpu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/goavcjmgp.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gfbgqwmoj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gshwbqjec.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gkfjgalwo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gmspnnisn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gfckzbqud.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gmophwfot.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtsbegtqe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gdwjpgwmy.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gprekmroh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gmvoyyivs.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/grapksuxa.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gzigcbshm.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/grziydavz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gjixblxok.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/ggykadopc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gpezweqrz.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/glzjaigor.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gfoniuqgk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfkjcraum.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gkgoogrpc.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gdfoofblr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gaccolmjr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gtrlqncpc.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gsovyrpqa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gzdtrsrvh.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gklmyolyr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gyvofdjtw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/guzhwbrot.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/ganglrbvd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gowijlmhx.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gdubwpeuc.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gvdviebqr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/grvjzlrpm.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/golxjmpfd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gigluxbcq.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/grvkzedll.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gfrtrsken.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gnuvekhsr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghqcnazag.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/ghmoebypo.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gyiiryrle.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gehzisrak.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gquvetrdd.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/ghrnohskt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gdaklisvg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gfulpefjq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gdhqhbbmn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guzrlwxel.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gtvqvwfrp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkifeebgw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gundgyxmv.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gxaqhimob.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gzdpsvlfm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gyqooqjve.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gqzzbsmnj.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gsfrggkbh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gblsvyojx.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gmvyxpcoe.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gvmlsrjoa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gyesdghqk.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/ghrzvtdrd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/ggbbxouze.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gxgrodwlm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gjlwxxeky.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gxphhjwlg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gljkqlzpk.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gpbdvgwsx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gpbwcwtle.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gbhwwwshf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/ghunghsyv.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gdnuovsvg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gdnlyfaqb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gkptkveyo.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gunajonhs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gqrzlgzrl.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gwegkssmc.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gtezausqw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/glzetrnur.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gsesbvhjn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gkxjzfaqk.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gplxvdcao.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/geaoxwrnq.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/giqsmydzb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gptpqhchv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gkmjcvbmo.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/grffxmhnh.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gyulhxeqo.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gqmnjfhly.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gddqpgtyp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gukuzwvnq.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gqmpzqfpk.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gkbioetgy.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gvvjaccbj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gqopsvxnj.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gynrlbgqg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gmszbtssa.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gzgaidzyf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/geqsclgtm.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ggrhlvhph.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gdlwgblmg.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gwvablgmg.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gjmihnylv.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gaqzcwwnd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gxprgzveq.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gewwreywm.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gaucmtsbs.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/ggyebdbbo.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gwqonzxaq.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gdbtcbbbp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcxmnsok.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwwnblcvh.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gkvhtgmkf.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gmxldebot.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/ginhvwmrz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/glkqqlheh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gexusxpjm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/guctlbevt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gqlkfafwt.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gvevqjsyi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gcqhkkxir.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gbxgkqbgt.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/ghwbbbrfr.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/glsthtvau.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gsgdjtxsv.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gpbdyxdug.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gqaorunlb.sHtML


<!-- 参考信息 -->