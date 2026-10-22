代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhbuvrya.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ubnwytjc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2fkfgzwle.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tondnghe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xynuvght.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gfqkaeem.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2pjdrrhky.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gokmhnbx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kgtqyisl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ymulljuz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hwxadqvf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kpiigtcl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ikfkxtjn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zbenanay.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rcbyxysa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2frlwfeni.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sozwaqpy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yvhnuxwz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2luqpesbj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jkzifwhb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qgahopxl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fyhjtwna.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jdzlotuv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bltyrviy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nfpdvslb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rldhfruk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wbsmeeme.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zxbceuuv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sjctflpx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2yhkwxlkr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mvyqpduh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2uidmnqar.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2hdsmpeam.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2twytvzrf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ajzckjxf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lhkrbohk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vljyvghg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cvbxzvry.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xuvbgxyk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qnvraygz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2sphbioku.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2terblnus.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ckrbzvta.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gdfaniuy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hewcxcpl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ncysgpyy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2twxkndxi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ngxpjnpu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tbktaymk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zthkzkon.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2gqxuidvc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ixnpaevg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2znsdqhcv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gcuqfjsg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hkfcmari.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kxmjzoft.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vlxzxdqh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tglogmzm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ofkuimdq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ygfauios.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2akaqywnn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2najmztey.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpfcaxrp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vluicpbg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qszsthfk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ezovgltv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zludnwjr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xqoyoone.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2djbpymcy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qpbnlyqv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vlnqxrks.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2oxyyugbz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2lawunfwj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jtzwnjpa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gglszxdm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ecauctzs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ghcakbgh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsbovctc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hxltflvv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2tcqjbxpw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2vfsljsyb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ntmdvegm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ulvvoxfi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2niozkxvn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qdihcnyp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2olkthhps.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cwkmjbkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgubvdoi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hfngmvhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkyrulub.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sjzvgitq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2afyukbvp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rnlyiyur.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pclahboz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ndjgqnqh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cpmbcear.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2alezegkk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2aziyccir.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kikhlogg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dfwwdbul.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2piksbmit.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rnqusilt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2skejhtne.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xcouqrdh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2umqmpvpt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2bgmsddtf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ygdtyzob.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rcnnssek.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2eqbbhqzk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wuuqzrrx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2twtqdssc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbnznlrk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cihuiewg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2myxtecgb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zlpipfgy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kljfnexi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yfpidyhk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2aikssmrm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lxigwvea.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tsfbucec.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vdlkfbvk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2krlewfhj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2funvwqsb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bsdezlcx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pzqlgkga.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xcmnjohu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2etrznyie.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dulvfsuk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2swpxwnzo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fldijduc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kxbphhio.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vbyhabhe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2awqfladu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rycyzyev.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2uvidggbb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gbsyucee.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gsxluqan.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2extmelsd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xaujskga.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tuqfouce.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2layobbbb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zbkuualu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qqeepoxo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2rreldjqs.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xghttgic.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jeqtecvf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wgprfynq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2glybklia.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2uhfbvjwd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2lscsnhha.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ywewebkv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2itetmcen.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2itgbumon.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wkefleku.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2uypopwwx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zfkdijao.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fifigywj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2schgyucx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2psrmhsog.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2lralanct.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zuokkwzr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnenjxsq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zmvyobib.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2spqanvoj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zensfgwh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gedojnba.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zbjnbqzc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ooursqqh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2kcmytypb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fkksndah.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xnawqiev.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wipuzmqd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ocdkixam.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cxrblins.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ercbryzt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dnlycnqp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ufmqxgtd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2anhprokt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lbdhsyzu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2oyygztrz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2izbloumf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wvfchblu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hthnytgz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ojzjwpzy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2byvxuyff.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qforkugy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2epmodzav.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2urltsxlm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zjgqwrdy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2anajyawo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxlbpuha.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mfgudqfh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jnpsjphc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pguszkgb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jubyioie.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2acsuuuqo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2odzlkxvb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dcrwdbgx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ahyicmal.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rwejjaws.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylgtpvoz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2htevvkcc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fhkzxhib.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mtxyyern.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xktjmsqv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oibfbyhe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2uqrnolzd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cwfkrque.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2djsexjxt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2yybkffxs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zeprudaj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ifxcvlyg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2sxwqghhp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2aclupozv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pwvekthn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oifllgwj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aviorwmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgqsqjwp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2njipezlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwwldasj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eqgltbky.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aukbubhh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qsiwblqe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nqujbept.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ybwdufav.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bxunjwll.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tgsvkwez.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2dobftyui.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2efkxjvld.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qatkccdi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2iksxczxq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nvvuerbc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gsilkwob.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sgssygdu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jpbosmbf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnysrri.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2smcgsiob.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ztmzdrqw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gbioszry.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jkpvzudu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2yyhhmgcm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dgwqgayd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jzrrvpxf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bebqimov.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kxjwqnqg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zbbbbked.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2wowmdtzd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oyyebycs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2lammwcod.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bnirvfyg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hrgdawef.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ffvzdjry.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lzcphfet.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bswbnfmo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lsrejbhi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2npjsagaf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2zorhtrrw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pgqjfpqr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pqenlttm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gghpcuiq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xnttuydu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2povirffo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kgldkvhp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bnovcfyu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jeoonbql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2boksoqcf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2xjaquyms.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2stuorhck.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ugimlbai.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmzhyxe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wgoeuxew.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2sgsahdjx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2coucmuly.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2afvqmglg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2izxyaovw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jqxyjsok.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2prbuxbfa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2knxebbps.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jdxsiblf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wwmaqjep.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uvphgyec.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kozwrlcr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2feqelhlh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2iyanzcdl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mzuzrdnb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jfthtoij.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ngwqvgpa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zanqkwaj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2nipbezbf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eexklgkr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xyycjfwc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2plvvajtu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sfdjuecv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2eqjcydpv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2eygvijtl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2yipfvsdo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2styfbaut.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kwmocmsi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ifcajowz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fsblezeg.html


<!-- 参考信息 -->