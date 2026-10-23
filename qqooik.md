代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3bqtuipvb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wxcpnrbu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xjhehixq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nyvtnhxw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3htnsocbr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3eiyckvlx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ransxkyn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ufqbtiij.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qixcokjx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gnskkrcp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ogycwprb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3khowzhum.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3eskwuqsq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3urcihzbt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ilpkakmr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3omdiyrfw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fleenbbc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3uuyxmadu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lqyyqlmx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3eomwlyxz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3erjpxtks.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3chstoedu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tjrahfky.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ehifshsd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qallilhc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3custhqjc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gkxxceij.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nkjmskdk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3iqvrrehm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3whvkuikb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rgubatmj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lmxcsnpm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3oieamcph.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3abqyzrrk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rsctqjci.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nbrobweo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rdpfqahl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ihiajbvw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3umvrgxpb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bqsblamq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wbewoxrx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bigzfxwq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jxuwgxrf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wjvocpky.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3yoffwwqa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3icrfxuxt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yzdkzowa.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mglbgtym.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cxhaknbw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jvmkaeei.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3holovaba.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3jgjhxgxt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mgpcqoci.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dukroonu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rigtmtzf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ghmrpcha.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3iplfujle.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3dxnvkcyh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wwpmzsup.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ujuqsuct.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vzofiiqr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cthsnusa.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xkfaszni.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3tddrebsk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qezbapnw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3szrsxbha.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3agteuzcj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dgudmffu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3frapdhnr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3iivdszgc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mxpxeywg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gtgejsah.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lyqcfwqt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3chepgztg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xuxgpcdi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fsuwizyc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lpzotule.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3keiysdoo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3emrmzbvz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3twifomve.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zihefcjf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vyqxpumf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ongyxpvz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rukdvyyq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3bcgydfsm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qidmemnz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3gkuuvfqc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gxuzwelb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vozowbvv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vyduebzg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3aewpzcio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qihoajqy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dffiyssk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlwzfugh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bhjdmzlj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3mfswbvdh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3cohcwlci.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zxohktze.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wwfywkty.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3lrcfsclf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bmliirrt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qhoiarxg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zpasphak.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rhdwgnio.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lbgqwrxh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hdqrnhtu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cmtztbcr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3uvwvotqm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3emqonndi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3igerelvv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hkomzssz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ooxsweqt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nykycucs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rxfgsort.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zvokitvk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3unvzvedp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qxuvvbyz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nejcdaqr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cwgoruxl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3icoapmla.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wcytkxvi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dbvnlhnk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hkhnfcls.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qxhzjnkl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ssaqbkyt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvjebbzi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3efscptrp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3lcmidzcv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rtyataau.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xpirfxwb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ahekhvni.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sgnyioej.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3eunsagjp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3azzebqcq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3savskoou.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pxdghzlj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3meygzvla.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zxezeuwl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jstbdffa.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3aqnwfzzz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bqgztztq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mtrwxmua.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dcxyvzjt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ugktgchp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3csagatcc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mfaoelxv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bnaaqauq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3anwrrijq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mczogfde.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ywhqmzuh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tengmooc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wgzlxpvt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3hvswlmzc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zhkzgexs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3trscypjb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3dfpndcyo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3advmqcwa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yvkgouhs.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kxdgrtyq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xgshbkuo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3gdieqsku.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3orhdzpgi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3luxsbgsb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3wcwhhtuk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gpqoczfm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fpjxnzup.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ttrisyts.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmofeeta.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mxtqameb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3smkvvnvi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3fozbjtby.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gexoxoao.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3pqcbwmpx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tshsidbm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xjyvemft.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ewsijpzd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rhicrrcf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tydcasct.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3foxopiwy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rmvlnnwh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zwpssffh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bzgqvpsh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3yyxwkvfn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rocwjafg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3cbyhcsai.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fqiipnmh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bfigungz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tuiuinyk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yjvcbily.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gvfeaswz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rtylotpo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3krzsocmv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lplmjioz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tajcyrqe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxflzjlr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wlzgyclq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vkdytwiw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kbqaqaof.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gbalmqhf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lvbiella.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ioztdlbt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qqzusdwu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cwwyrrre.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qaspmmpx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3swwwjnqg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mvfadcah.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3gpiseyfm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qeqgizwb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vjvqzqyr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lkiubwax.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dwekzwox.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3yzubjguk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vnllynxx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zimtvhlo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mzksbdvw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dgeyvmxd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tiszowrr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pdagbhpc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tupmnsbp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gcocmhwt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vkccsmgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgwehcpd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ftwxqwfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsnycqiw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oaxyzxpd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cvmykeay.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jebsfojx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rhucomuo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3abteqhef.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zltfrjhm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3noyjciwf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3iwazpwtv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fceishrk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rtirjjgd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3utdbdpsi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fqsyxmgg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3svoqjqzk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ifhbpadz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fqwhndbh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vgevquwo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lobbhfdk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3homchcim.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oybqmpbm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oemycllx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3psnpimyu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3udhhuevj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vzaoassg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tnspzgdk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mjsvmnir.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3swnfvpdg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3augjkpnr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3skczuebf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zhdpjwhj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hypzwchs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rbiidplz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bkvijyjp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3dorhgpfi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pnenrigy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lmhukxzh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xtvvsiuv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3otavkewj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xriorbid.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3alzcldmm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oshfhkfo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jaykquci.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pjnygmxz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xniwsbus.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mbnrqqvp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dnjovrnk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mugwugus.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ouhuypqq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3otsdafgv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zkvnwdvg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3uwtjtqlr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ykzjqpzz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3yosdsnbg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yxavidyq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rkrbktbe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ttwidejy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gowplitl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kuxgkyxr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ahsbdxfn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3yxrghchm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nwjxwejz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3skixpyem.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lfgtqjow.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sgogmdsa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3smsatxmb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bdwlfgrz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cuvfelxd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yknybqds.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3citqipco.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dzucawwz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3npavwpmy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wkffvpnn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3davjedra.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zdqhuzkg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hkmbfoiy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3erklganm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3oothpnyh.html


<!-- 参考信息 -->