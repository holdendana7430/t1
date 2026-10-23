代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgwsnove.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3cltylwhy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcizheuh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3iccgkcve.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3cgqaycjm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ybdmfjgo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3anyhvwps.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3igdnjwht.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gsshqsog.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kisqzegk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zowalwml.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bfvfnsek.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3faaqbgin.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jzinopfi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ervyvlev.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jrxkxune.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bviuylgk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3geaweppt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ekdycfmv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3twktlsls.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wmwwquxm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3reganppr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3bikyuuhu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzjtomgs.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mkppnzol.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kjnoqfzq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wbzizugz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rfxmpacw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3emamqfdh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3kmlxirqe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fefsobpm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wgxzzpxk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rvmyngow.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eojwbrxf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eyzofgtw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bghlnkff.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zusiofdv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3uyaxmnmy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iagrtlnb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3abnvprzh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ffqiitek.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3izyotvsy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vmogoxjd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bbjvkdgg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lhswkyqw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ktkezuaz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vglxtewx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ecwexeak.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3brrxcfhm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3axrartna.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uxbkadby.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3sitqvavc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gbfpklkb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ubqwnzig.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mnbscokl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hkcviggx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qbdeazvb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zntmlqbr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jeujnssh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hzqrvytq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nicmanjj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnqodigi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rhggxbji.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qvjwaxaa.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ojtuvhcz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3axuotjwv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cydhpoxk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wtbgpcwb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mghqwxid.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wynlgcqs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3puwbumtt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ekmpqpte.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mtbodeno.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ktscmjbd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zumlxugz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wdkoxcgc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nqggxriz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gwjjtoof.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bltupsmr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3urlrgprb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cyhwrslc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ismtlrmq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qgdjsddr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3paxvdrfy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3waecwbkb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3semguyjf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lodbhhow.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rjpijgvw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wpnqmhyb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3hnsqiyuy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pwqvpnnr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3egiijmpw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3whkarjik.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3erqaebkx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vvkyfacb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lcnearqv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ejnlrtvu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3idqnicvq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3irkqxiyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uaoetsss.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xwxopoac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stinjgbt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zvjngcgw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3erdeeloh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wszzomjl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uhkquslb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3eaenxqzf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3acyerrin.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rgqlpgfb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ctllidmt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3skivdjcb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mvhdlokw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ojbxiryz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3znkmnrrl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hveeqytl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xpqxykth.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jfllocya.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3knajpezl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hehzbmnx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lpwxghsa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3occahruo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xfkpkjrb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gzfmvmfc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3leaklyah.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3oetxakov.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3srstognn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kvvuijky.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvglkmud.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3elzudjzn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yfgmglix.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3odcnoqur.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kwvqqkok.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3oxokuxwi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ijikgzmy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3kwzjsyvf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3avzgtziq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3nrtnkvtc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zmawvuhi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hhrjllkj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mlrgpurj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jlvrnsjq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rzmqmqsa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3doqbiyaa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rwqpkxdr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zpneqyki.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jbyuhvgc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dqukglku.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3usbzbzye.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jdvemxam.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3uhvogvdd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vjjaioij.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3icdvgqvh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3uiynyeok.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3cikfuzdz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zbwujpek.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pjkbwwyh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qaihbylq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jgrsniwi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ilsguktr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3atuhndzn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xzckkaah.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjaqeygk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xlxamhkp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3eaeziuzc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ttunmlws.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3koyicusm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3erchlnwc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3btqidfog.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3gipgxmvf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyakwtqc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mbbhpzsx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3bxkpvygu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3onwcwmoe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hwflbedl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3girdxwjb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccamzxzn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qkbogrmu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sqgkhmzh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jftjnkmo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vnvjvvol.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hpcsecrv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pdcuvdze.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3gthetdmz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sksfnrzg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qtaahgzx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ratocabw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3itzrkptz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ajssdhwl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcqmjzti.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uzwdvtwc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3owadljwx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lvkeghvj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3huqwfkqk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3slfkuvmh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3qwkcfkzp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ttwyldhu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3clqnhusp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qauypjpl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kphsmtod.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tznketnp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gjgemzlo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hmpewrkx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qswoljrt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ifqflvry.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vaiweqnj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hbysnnte.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hsadptsr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3insuesvn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hzocuqzp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ibfgchaj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bcqeqrdg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3reygapqs.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fdhkhrrj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3knbnvubx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ywmvpioj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ggzceojx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pwnsyfbi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rvibyrjv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wevblfzy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dfxxepyy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzqfqbhf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jrvrhywg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cgalbnmx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sdftrbum.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iilvktaf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fvusoxpc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tsqtohvt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fcersupp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xyeavogc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhpqkzwl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wwlpbkuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlouulnp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ezejuqvc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wqutjhrs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xfvovjvt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vitxhbvs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bpdnxqzs.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vodkrrfm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qtpbpwjt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jxmeqovr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jpcxdsyy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fpuxjhuq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lashzmrx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cizsowlw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tviyitkl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mctmveek.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gesgvmeh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nxkbalvx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zzovlyjs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wdbwuzlk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cudvziqh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ostfhrpx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pkwprtfh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ggyshcry.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3tsiearsg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ahuythzo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uzbcyirj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mhdnnrjy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3beznmtwq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vmbgoulp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vxnfxpkr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3baolaaqg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3agryaaea.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zphgulta.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cjizqoeu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bejheqmo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ljpcwxip.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xixvioyb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fydhptgp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qmanvbga.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3sopzjhdt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3phporwym.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nsfujbpr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bknzznch.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ezrqhlal.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zcrudqbb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hseguzmg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ugwaijdb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gvtngxkn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eyahtxja.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mwuphqnr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kxlcgbxe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3cpyzrvtk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3azwbrcti.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kjyualhf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jadcrwbd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3edcaqmig.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qgbssrmk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ggtnjkqh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3papoclxc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3knsiopeb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3fnegbmvl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3arcdxrbk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fkcloura.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3afstawka.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwfxsuhq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nngucrqs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fffpuxdt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fuwhvsjg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vklwqvgn.html


<!-- 参考信息 -->