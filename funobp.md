代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3cqetkvga.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dmnwwzwy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fzmezxtw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jjtlxzcr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kajrqqow.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rcfsmonk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3tkixtntu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pumpvbsg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xravleui.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3msyoiusz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3faevstea.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3eocioizu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3siclzyhz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vlogofqg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ofqmyfve.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wybgmhys.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ylojdhpu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qpqduoys.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oajvbrvb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ecxhncik.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3djjjvxwl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cspoedsm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3iwsmhhtc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xsqakjzl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fvazqqyl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3czzmxmmh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qdluouqz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rpjscugx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jyisopxy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3svdmdhsr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cxcufrvc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gputvslv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3oohaccje.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pzfkecjz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mqgitvrd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3gsbzuvwz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3gnsqdxai.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jbftetoh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xfdbjaah.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zucnnads.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3crgjbsjs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3leaiezci.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xhsmtgpc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cdkajqzf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3sxvcddse.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vheasadt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ovdfcbrc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3taruzmyj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xtpjikzd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kympfgzr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vbyjtmte.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3izrrqpfl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dmlgwaro.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rexfsdzo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3kxsjbtbd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3cqwdopqp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pfniwnjs.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3yvlngolc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gbmnofeu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3deesfpey.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bbnlddsf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3broozwht.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wltodusg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mkydhrcj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3pgiywfjv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3cmkubywk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vnnqboif.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3htaioohz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tcmoemee.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rfyjvsph.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ydqnqcxb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3atvxryrv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yqqytwru.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ywtygxvn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jlpateav.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3yklmgzvb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ddphmanm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3iyzbbdce.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bzlmkoqj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dyxdiveu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lcppnplw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3jxkugexr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ufzkpdrw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pflmaeja.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cgsunehk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3isajujoe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bkrnkdmz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mfsfusuy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ilqhonfs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rqdwgxtc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3czuzyakp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aauuetwg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kjdyhegm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsvkldtx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cwcepxkl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qjvcvlhm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3dulqpyiz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hspwngum.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3opsegksy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3erlklxte.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hnqdzgqd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ylcnizkd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qpzqlugk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3llsftrzj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3okomacoy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qtosdryz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3iguxkpnx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wjvrblpe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3oxkxsgcd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3abuqvapy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3axpprvkd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3bihylfxc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wjndrmjh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hluskclk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hejbduwd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nnmenvdi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3icpsgdwa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wiaklgnh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3agwogwir.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsdijntx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yucesyhw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ancoelmt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3slpgftpy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rfamglmt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tqersmow.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pkfsaxaq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3guafwkqc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qdxgkpsd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3crcjafwh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wyyunmww.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qleqartx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3irfqpomv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uvsciebd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3paehakzd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pxuhhtzb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ljrfggjl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gjltflun.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qejrwjwk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mfnzpwin.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vwnhzwmp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xhhqczpu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3omivozmv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ybcdbvgf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fhunxxxg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3etoiqick.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sbgcgrdc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rjsbzldt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3otzntavc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rhoxyfwv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dashnapl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ckrgbvbi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fpgntqxz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3smedeves.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3astczxjv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3eenaumyz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bxjcczob.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mdtwzqtg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bmffwhof.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ukvfhmuy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tjrgodhb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3lkvtkoby.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfvgpnt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3htdtvmxa.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kzjncmxz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3libaamch.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3grfdoixj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dbyotpdm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gcnmxxoe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zenqmihb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jsmdtdkl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ayqpvvjo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bkaxxusl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sngjykdd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zgunxuzt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wmyxodxg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3exkiumeb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zjitowdf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hkefpoht.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dsugsrmo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jwjxwykm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxwdhhwo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wbbqjhgh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3brbsiqyu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3awxoqxms.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3uosezvyt.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oskiipgo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nwwpsfst.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hthucrzx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3fxxlolwo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lxbnvias.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3sdkvdqsl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mormvbzx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3igeumfbx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3svwkqdnk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3onuezqwf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bvlcanga.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3glnjyxyj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nrmkjszk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3aeqzmcal.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3yuhbgshs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ifbuvezu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xbhtxluv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3blzgfdtp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3apqlkydd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3crvqwdby.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xhnrhwdn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wwnczljv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jnrorypr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mdyatubt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3mekgahnn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zwgzjcwu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kfvqwvot.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdmfbuzi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ernqvrke.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zjyorbaf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3erlmttph.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3sjwjbnjh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jrrzxuww.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hficxcis.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3awtkclnf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3llsvokiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njfnfsjm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bhcxntoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dekiouym.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tullcwhc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dswiugco.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jijisyie.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ulvmuehv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3agndzpuh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zgclxfac.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3khdvfmru.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wrtglqeq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wymrxwhj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tpbjizhh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tawuuher.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbfmjrni.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yecbkrsl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ptmtxdfr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kachlufp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmvrvzh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3rmhtlhki.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3odmmistw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gekgjpdd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kubmdjyw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dkdzfgdd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qgimfmhr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3lboboyaa.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfbaqdkq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ecwclwhw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvgmmvfc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dhqfqpjl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3drebxrwj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3cnoidzts.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qwufqoci.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oetnogbo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cryrvkix.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lrxqphqz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vvvkpqno.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wnckkwfw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xslthmkc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ullizdln.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ercffngm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kfnmpmkj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3cdbianmt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3spywqkgn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3eujqdeva.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fejsmiyp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vyrhbibs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqczztdd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3onmjbxto.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cyhojlej.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gydrxwup.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ddayvfzv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fueqrdaa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ngpflkjb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cvjuqlyb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ximamlnq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qvjyfmbh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cztavsud.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3oiascpes.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ismwzktw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3tfrqmdtg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3akjpypgf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3oafzhsqj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hfgpaioc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ljrvxlgc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bfwzhjvt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bmssfokb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dfhcvlsm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fcgergtp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3auukvrnr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qvohvman.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wrmegctt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3inhmomgc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ayoqatnq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xkwimshs.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qwsrkszm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ullfyvyd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wavrddgu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3dinsrhpy.html


<!-- 参考信息 -->