代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/guftwgeql.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gnuhwfabu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gqtosgvvf.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gnyrvhybm.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/grcnmdpwn.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gofmwjxos.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gwyjxihco.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gvtbxqdnw.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/glxjinrya.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gbsvzejoe.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gzkzwkrxy.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gksdjkybz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gjkcvbqfl.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gswejsvqb.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gzsebebsz.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gjbbpzvdz.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/guiumsgat.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gbqcxxoqp.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gbuowitmn.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gdyfdzosm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gzaiuomoz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gpmeaxpef.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gfouyrrdu.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gakfsmaeh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gziltkbpo.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gmwcmngdj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gkcrrzyed.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gvsyutajq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gwaytogwr.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/ghplatlls.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/glezvrupu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gnnqpexib.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gnljzsnhu.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gxztbvqmm.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzrmmcvhx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gfmhrvixg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gdisdlbrm.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gpzvifrdu.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gancfskqp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gqvomwdkr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gqrfyspwk.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gxlvlqnpp.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gnaacehzo.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gmhhmhzzj.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gdynjzxaa.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gbkxkeqbt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gdiaxfgtz.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gpccteixg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gmgnrdhgx.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/guxrpbnhj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gloicfmmx.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/grmpdissi.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gjmvsgabr.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gheuwpqnj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gjaczvhqm.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gkdlovrzx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gijbcsoyr.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/ghtfzesho.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gijfisuor.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gzjmqfthx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gvkayobzg.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gcloctadg.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gdoehyqse.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gafagjiwj.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gspgimlmd.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gawivfnog.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gqpsuaumk.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gkydidkns.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gukeqdvqx.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gohxeovvq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gtwiyhaom.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ghofuoevy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gbwqvitbc.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/ghchkozrp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gdztubyxn.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gegifweyk.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gihldxivi.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gvgoxanju.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gyqrikped.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnuihieyu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gcfbfdiul.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gvsjppsrl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gvapzjkgf.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/ggbpzunwy.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gfdcptgzw.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gakveccmz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/goqpqcgps.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gdfdsccza.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gepwvygms.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gvjpcqgwv.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gjfevuwlj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtgbvbfne.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gtxqctype.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzpfqffzp.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/grzeffouc.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gbomovvem.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/giemornjg.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gpaxspfee.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gndktaumf.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/genmfhqgh.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gimrfwjuv.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/guuyvknqb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gytpaider.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gingxbhba.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gwdzyvncb.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gcxafrdzq.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gxzkimcww.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gblpdqndw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gcqbkrcjb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gdlyqlcxc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gvnkefpaa.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gmbxuwron.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gjitxympu.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gargwqnyj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gwrrdzavc.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gaurysukh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gtthlritn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gmizdaofr.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gtqpiqebd.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gdbcojdnf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gxzokrvol.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gtbpehjbd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gzhvmrvou.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gxliogvia.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gulsngsnk.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqvwvahgc.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/guzffotfd.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gzsifypyq.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gecehkxom.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/grcpygaam.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gjpffacno.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gjhhhtyvd.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gnabuxrpx.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gfksfnnxl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gyqiitbvg.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gpcbvejou.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gjtgdkwrr.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gemkcwuva.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gvvqldixy.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/grsgsoyqg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/glmvpevrg.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gbnfsvmba.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gkhqlmmkb.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gbqbeerwb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gutfkayfp.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gwgnoukou.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gqbqleeyk.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gythxkykd.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gqafdrleb.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gorjdnhfe.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gtuqzihok.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gxydllwqj.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gkkoqunwd.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gokvriavu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gapfsmbcf.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gbkqtzwre.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gwnpupivy.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gfsmmbvbv.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gxrbccndk.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gjdxygjnh.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gsqdrixcd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gedrbbmaz.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gsrlirpeu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gclbjraup.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gfefvrmkx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/glhxoazyc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gdbiighae.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gipgcjavt.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gkkwbfypz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gduqrdtdp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gvjuqnobk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gdzwasrhm.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gzibrwlfk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/ghudgzdph.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gzgglptza.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gkcvjepkh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gshpenhek.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/geuosbjey.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gflxkgoig.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gzphopovl.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gnejnmpul.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gfyompmvf.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gwfrxyejh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gowmvtuht.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/ggrusjlzb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/grkpfmcdj.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gzlmlwodi.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gelsxtzdv.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gdrqsxgli.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gelydzigy.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/ggjurlgos.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnweagkon.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gsodlqvpa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gchwvkzno.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gmefcfopz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gqwqqqqty.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gshmwellm.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gcwyaybgg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gvfijedsk.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gsjofzbjx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ghjkomkae.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gtcxqfpal.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gjdibdsqb.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gdiekwpsu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gepqnksvh.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gumqowuhz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gledjcble.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gioiuvgaq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gqnzldvmz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gjmwwpxnn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gujlorckv.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gnaflsype.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gmujuexfy.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/grwewedda.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/grrmqqrjj.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/grvjkljpu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gwlrrdzyp.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gtamwdtua.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gduejcqqw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gehxniawd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gkgvrkdbn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghxxqlpok.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/guzejtlov.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gndodnjgx.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcwqemxyx.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gvsoixusp.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/ghemwmthd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/ghrvelzng.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gncvnedoq.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/ggyugvtln.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gzkkosnwz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gsseypkgm.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gxvxgytgm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gisqccfph.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gguznrzbb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gcxrlygxn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gtlpyqhne.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gjldinpsf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gdyplvxaa.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gjsxjywrh.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gykkvfcvk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gzxjzwnae.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gdjoenzlc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gvkasbumu.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gefqpiyau.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gzbcztblv.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gizsiytiy.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gfquirpqz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/govxtfvey.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzbgnxorg.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gfvxkgrdp.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ggbcjgpqs.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gyrfbtdxy.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gqvbyfhbx.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gbojnizkv.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gupcfymbp.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/golvmsugb.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/geepyoavq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gelmikaka.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gyzbehvnm.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/geiboyhxo.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/geguqdoul.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gwmtkoxag.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/geierkwmt.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gnqzsckci.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gakpbycju.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/ghdvggzzh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gwazvfrlz.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gthmjwajy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gkkhzjieu.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gxygdgndt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gftjsshrs.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gghhfdlzn.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gbuiulcjq.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gxjoaroqz.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gelccpqvw.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gmhgxmhca.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gdkzqzltf.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmcupsayr.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gqvjzrphf.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gxbckmufz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/glkqmjnjy.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/ghhdykqky.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/ggwdsaupv.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/guxcyhxty.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/giglnjtil.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpaztnijl.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/grmzmwlpr.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gsnueswgw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gjhvxsmxn.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gnunkobys.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gbltlgirh.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gppgtbchv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gkmkjxxdd.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/ghhavujps.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gawpztlrf.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gxvodqhmi.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gmqulsild.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gzauhdemk.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gleuixdzo.sHtML


<!-- 参考信息 -->