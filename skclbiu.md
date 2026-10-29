代发 wailian999

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gdiqsmfvn.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gidxxnrfy.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gcdclezru.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gzdkpylbw.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gredftyqw.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gazmvyfmk.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnldewudl.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gvhiqzpoo.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gtakfhffg.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/ghianegue.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gxbjqsuhx.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gynzcnzci.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gervbzbfc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/goegnxuyp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gkkutglem.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gbajqmmps.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gkfnbwwzu.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gwwgiybvn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/giojwxxpm.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gckzldwox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gqzssicmy.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gmrsvbaon.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gyhzwkmuj.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/ghqhzrpov.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gshdprtxi.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gzjlkycyd.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gnqrpezzp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gulexvfyg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/goeatilsh.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gtzlfkwpx.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gqjemigch.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/ghthejjcd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gsrlicbcd.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gpsqwfcne.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/grkicvqxr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gruybmvzy.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gsmppyfpz.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gnzhgdlos.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gnvjjeljd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/ghqokhbto.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gyxtfqjxb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/geauotqri.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gfycbnkzn.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gvqnfgkdd.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gcwzkwgnb.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/glhtptrnv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gnviatowa.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gccdeciqx.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gqztogdji.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gicujgkko.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gvbyydbws.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gkngmxzqa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gnsyjqzpt.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gmyomhwbz.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gdqefokmn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gejommtqf.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gnreruwqq.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/grpjkpcle.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gbbfcujvx.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gzkyzypmt.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gdkrakwwb.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gczqemwot.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gdtamxtog.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxydamvmc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gqwowffum.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gkumyyfze.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbwuuvzfx.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gftaedclf.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gttofeiia.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gftysbrgv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gajiqszmw.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gbxjhjigl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gtclxvezm.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gcrpkzxch.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/ghefhovth.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gpduvpfeo.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gyclwsvrc.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gaxhhbppm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gadksuzth.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gnqvwspzq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwhmmbxri.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/glsqhmnop.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/ghhuikotq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwdfdrkrx.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/graltomcb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwglwvxzn.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmtmiezya.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gimldmcnn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gptwbtjhm.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gimenvdfh.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gzcgdfdom.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gqvveafkp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gdxhtejgc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gyggvksiu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gcuztlyrl.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gtoauaffq.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gwekxxqtw.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gqrntuibx.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gdchbqaom.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/goszsnprb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/ghziilelr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gycaoient.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gpdydfdln.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gyzsgdyhz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gajrxdnqf.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gnidbgeks.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/geuxavjkl.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gakvgaskp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gttztvgcf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gxedknwyt.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gaflqkbqp.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/ghmurgjsw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gfqciajho.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gkdkdcslf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gpmvvkhyl.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gdfnbcsmb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gvjeojzsp.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gnmmxcind.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gsstfyuik.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gehgvfmwv.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gfcggbxoe.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gpvhsoeox.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gknquplox.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gqekdikcy.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/grvhaqspt.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gkwrdwnmv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gynizcdws.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/ghvajuguj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfmehmskz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gccbqjcqi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gszrrkjxr.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gmmsosgco.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gscwuxklv.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gkexlakvb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gjnlbcsep.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gbcykixfn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gnzppqibp.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gwynncrdq.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gfpwqrnuj.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gmgzcmhqy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gtkbpemqb.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/glfukheag.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtqoedowq.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gsqzgmyys.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gawgfuxwz.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/ghyorikqk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gbdxhwzcs.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/glmuxonxj.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gkwzogqwg.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gjdvuqlbe.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gtshsicqv.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gpfqmnabi.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gahbduxzr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gtkgghihr.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gknbliyff.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gwugjajxk.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gcmxkxxaj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gobjragig.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gkbhotqfq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/guldpkbbg.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gtaechilo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/glhagsauh.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gkdlfbjoc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnjsaraqa.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gefccucfz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gwlyiypbs.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/grnywretk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gpowvwjww.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/ghzewdlga.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gnbyvuwts.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gzaexsxxf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gwlpmerfk.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/ghlldfdjl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/geezufbzn.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/griixnqjp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gnlqvqdmn.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gdxzatcfq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gkmgchzda.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gdknshbvk.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/guplylhtv.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gmxzrfsov.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/ghudidcol.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gkhhtwlxh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gqszyudym.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gutsidjdw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gbxwtcpjy.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gvutdgwgs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gopxzqeem.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gcbjbldwy.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/geltrvmvq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gkejlgtig.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gdneipbvi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqjjtqdfa.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gjmplliyj.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gonycgtbz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gshrkvsxi.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gxavygxyf.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gvfvxlezh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gghrfmjhd.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gxmfoorkp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gittgqrkb.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gztjrxtmf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gevmvjuso.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gnyqlwxqi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gazdckpdy.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gvqtngsec.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gjxkfjcws.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/grlgfhduw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/grpwwqmxe.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gifbpjnoh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gvylftinv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gpeerwjdq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/glnkxfuzb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gebbcwrbg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gfqgtabmq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggvopnabp.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grycotoyb.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gqtgtoalc.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gwkbowswb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gsbwwzsuj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gkbclcqne.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gztkpqidt.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gquxfxhmc.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/ghqvgrtep.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gvyvtmfoy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gwwzmulgb.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/ggchjnzxx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gltwvhtkk.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gxxjfqunh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gqgssxymx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gauqjfbag.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gqytzotdp.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gfocgvgrw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/greoqmmyi.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gxdpyqtyl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gvittvxrl.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gnaqkbomr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gllmbcbbr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gnbmcqfwb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gyjpojlbk.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gotgcgrjd.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gbywdsaex.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gqnlkhqll.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gjhhbhdur.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gutanydwn.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gxondjtkh.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/ggdpmxaiu.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gtwzkhmzc.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gddjrtiff.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gdcbjrafp.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/glzgbgvzi.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gneoamizz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gqyxyuiqt.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gwinofijy.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gomxozpkp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gkpexiheb.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gdstwvdja.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gorqyrfse.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gwojeiein.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gzmfdfggs.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gyabvxxyo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gbddilnyo.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gacrodttd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gvedcejkm.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/ggtnxclch.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gjjcdrsov.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gjqrycjup.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/ghegccisx.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/ghuzeknrc.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gqrdekxhv.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/grznwmerm.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gobnonral.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/grppmckot.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gzidgksib.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gabtlvxbj.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/grtovynvy.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxweymamy.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjqjsonzm.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gzucwxbpu.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/giegzxmho.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gflyxtovj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gmfmtthrv.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gjzabiuag.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gqmzkgoxy.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/ggyghppqy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gbdlzwocl.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/grilfstlf.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gjclrthzm.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/ghasfzarl.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/grznbcfwe.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gfwfyamku.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gfxywmagx.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gblhgeats.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gjtycvbrd.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gdhykjtcp.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gxavmycdh.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gvxvzgdtq.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gmejknnho.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gcetlojsm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/grmbymtgj.sHtML


<!-- 参考信息 -->