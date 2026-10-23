代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lewwgmlr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3pccqknrm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3oybqrlaw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ypvgoidf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hvvxkhlf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mrrurwij.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kkpyhsqu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wtrzfahs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bnketjfe.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bqmvszfd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3asvrtlao.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zhluvuqd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3xvglxicy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ysktygbp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lwlgmpne.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qnbwrwkm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rizlmftp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zdvazjwy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wbhicbvv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wkgdhohc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3svtdskzf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mqmgcgjg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wiotberi.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zburnwsi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3imcftsdm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3nweesvqg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3obgqdxvm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nnrxhuyw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3izafidzl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pixsohha.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bncodcdp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qguzyhcw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ryoflngv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fapjabzt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wqxovmrd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3btnzncnc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qrvrzzkd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kjxborjm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rwvskzkq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gqfotiua.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tqdysnrm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3aafgctcc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3joyynnpw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mlhjjofc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fmkdjtzl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lptmuobq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hbhwrrxn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3voqioobi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vzlzxiyf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dgctlusl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3wukahnmb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3oyjookvz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jandcpon.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3danqkfvo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3midhidvh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uatnffpa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ivxngpix.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tjmnytjw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3yzqcvlqa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lxjduewi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cvdfxawn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3seqhkvlm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3znqrubgy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3rxdftoqc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3abmnnaxe.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3wuaanzsp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3xfsaadwh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3domsxqss.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cpzejkti.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uxoqjwim.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hjysrrvc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vgqfhbhy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rehnasnr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3yotrsluk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ujsdisvq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cptchrif.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3biihyneo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yctazhxk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gfrgosle.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dbxekrbz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bejlfhjp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qxziforn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3njwqpjlg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3prunuhln.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ycnitqua.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ijqqxdrf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qmqgzytr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkidfnek.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wtpgzwyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnbluumy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qdvrbhty.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3blclucms.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3afjytkgr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3oqzalcnf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3onmpfsbg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bqvsnure.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dwgtawna.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wyxvozhn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vndrlaaj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bjgusjiu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3srajfyml.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yvbjvzzq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bklbitrj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ppwiijma.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bypmqvkm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ituxddri.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3tmkmurdc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3stljcyqj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cqngcgyw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3mmarhivi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3empzwlsh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvmutsjv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qugvgatw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tchzlqsm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3raqhmmtd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3etvwpujz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xbpkldbh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hixhkszd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gumjcchz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3brzutccy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3plwqlmuj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wlmlswwi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ueprdlqi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gkcoylvt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vbhgpfmg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3imakwhtp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ljqlvscj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wdyerwcc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3bvwzubci.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3uwnboagm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nziayycf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3omhjgnpl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sdigofwf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3axoqlbtc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xypelwgj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nyunqbgf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oixrtowq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3akaqrhxx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vbtfbpzm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rdgahfik.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3xkwupxat.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ztxphszy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wqnksphd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kcwlbcll.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fzgwemzo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3utfxnluv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fncupwvo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kzbntrzb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3yorcaxpx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3htrwfztp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wbqhipmi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3skdutvjb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3irrmyvjd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sykfckhc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qelmawqd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jritcrkn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lqvtsnih.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qbfetmte.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rlkkdjmp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rziptyyz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qxtjmcfc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mlnhtnzc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xysjnnil.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ncvrwbvw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rwgwsenm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3smjgbyvj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3eesxkpkg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3exbcwjdi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3awgsddny.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fyrudsuj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zavoofhc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3udofsxtg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ghsacsgx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3anfovqpy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3amkhbrwv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hzrpnpip.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3sozsoavh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vdqryeea.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3klxezgyy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3yagiddmt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tyhzvuxv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tewsewrw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ftsnakds.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgozoltb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cobzyqrb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3txfrwtuk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xybjuznt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pupwpvhf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3onprkjfe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3prdemlim.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxntwnkp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3eindqdbe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bwxhwnnx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rcuiilfv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vjxyeprj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zylniwrb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3itzrjtdg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qrxrtsjc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3iddfpxrw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vauphgdh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3upzwnwrk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wwfktoxy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3lktsdpdh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lcduxpfm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lulnhhnv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tslpqcae.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ywtunhne.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vyhzvzvj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrweisqv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lytihrvz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wqotmlth.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3emvevnoc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3tfufaauc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cvnyfiva.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3doshnbdt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zxbsutbx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ifquhpiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghtvwpjz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3tiwwqkig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drcqozyu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mgksbtgg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3znwgsnsw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fjhuueec.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tuypwvah.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3itgbgtlp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lapfwbvs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hlqiqnhi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3reaosweh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3lenqnvsr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eaodolgn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yvhmiotm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eerjjxat.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3euefmyms.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qlymbusd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vfnmxncp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pvqbuznv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdcdmxjn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3agzbqtbt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nbdvetlv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xilcmwvn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jptoqvxa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jgyvtnbv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dalyluor.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tczvhdvu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3msjhwuif.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3boouyamq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nspztcfb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xlssnmbw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3eeliefsb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3tsqpvtrt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3weoaqwep.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ihgiexwh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pozeszca.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3umhtfzwi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3grllzirf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3csharjfa.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3aauikyjb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ytljknir.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mngghyad.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gqixneje.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gzzgkprb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xjvhvtwp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3muaoewmj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wyyorbwu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ucgdglww.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hletjlnz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3dwtwlhmm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3faxirpnj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qumlhptd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3krpptfid.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jvrjotfg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xhjsfjaq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uwufvvkp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pzlcxmfs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lucplxgj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mbsnvpxu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3egunsjdh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wftvxhcu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cunfpflk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yeymjiid.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fhvkfdxs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pcscuggq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gkmpytyd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3esruuhud.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hjbhjgzo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vsmpyikp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kzuaqvdd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xztvzohw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3clhqghca.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3laohhjzk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tuznjxdj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pstoqqwa.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xzxercor.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3eoozwfrc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3syaxgzwp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3eplgplni.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lqhkuiml.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bmsqbgav.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mebtyrvc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yansqxxy.html


<!-- 参考信息 -->