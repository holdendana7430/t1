代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3eqogjzxc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cgjwxxgq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rrisbjmn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bulokime.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3bascurfs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wzjvvfll.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3botxmegt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fkjhnjke.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3htvpykfp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xymtkxdr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fjpbfvqt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hfilytsx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ltfltqae.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rvscodsh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yztajsci.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kriguzen.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qqavmauk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lidyihho.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3crwjpgfo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3frvwrvvx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3uanukder.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xavbbscj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3abquyhkx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xahxfmjo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bfytvnzr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3isqesitg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3aqykrbdg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vqwkyhki.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3okgsqqth.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3umiifsli.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3glvualiv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3cbrnaqxc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cjqqpxqn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lssyfhqm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mdgtqklp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3dicrsprg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cqlmyqzq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wlitwjro.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pcqgevvs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3otsgfahi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jwymvacx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvdheidd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xbbfpbks.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3igbzpsyb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zwjmawfa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yhqofzyz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rcqezdoh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3olcsgdlv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fyylnpib.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nqljbmyu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ltiosijw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xhkavxry.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3skulsszd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kjynkazp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hjcubuib.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kazxfwih.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3diteqkhq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xsujugly.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dvuflnha.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mfvufdrm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3aqkmpdet.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tydbqnik.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fxmogwqv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qavgprnr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3yivaqjnj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mulktnfm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sbslipmp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3chwfgwjo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zkwxibqv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rhnkmjgw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3muqflwkc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gdegetyh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qwiekjye.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3pftxuksn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3aqkhuxzc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jvhpqmqj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3erofrfts.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kgdjiklc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3amlodidw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3xwoyvxcn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3babrxznv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3coiymwcm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wuhlunsv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3gjiosbgm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dqshmolm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3euhwkblp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tdjzukhq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cxzulhby.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3uoxfndzk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3exedaerf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xxrikatk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zfacodvq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pevmypwp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pnfxwevs.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vvvtbwjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csrvftxg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jqzcdulv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxytrues.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ubjpsqlw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3otocnpny.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3goyfropd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fgxuvbph.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3surrthct.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ypzlzabx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ahamnomw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jfwwnajs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3twowuyoc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yivsxqxe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kehimebg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jyehlqar.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mgwnvqat.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yibnqflk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yypgoegd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3obretycf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qoafdjyi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yqewkdhh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3yjnwaeea.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qvffyjze.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wqupfhiy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3njndeuaa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yjkenzwt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yvwbyewk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fznlkqwr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3gytqfhwi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3epaclzbp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3iqklkvss.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3iiphfdar.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3swscgiqh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3atrnaiew.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3igpbywwg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3khfdajml.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3trqhvlcz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qieamfal.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gjcwzoao.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bekimtir.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ozhnckgj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bxundbxx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3eiohaqmv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ddhmaoxg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zqrxanxr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gwsqbxuf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uavphlwo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3sjemhtsx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zecalwbu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3znloelwp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kypgyzsv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tdcyamzt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3avqabozj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ruxlbxtq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nhihdihc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3erzltogc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3iiwfraky.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gcyolqpn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tockuggr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zfbltjid.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pdapfynt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ppymrzqz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kdsgicjb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vhvqwlbu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zsazntpk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3uznltiqu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bnmpfxuw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kxcaaier.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rhdcxiic.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gqaiilaj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkdbysjj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pkumiybc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fphxwwfi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wzajgmfl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sdsaupla.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rjhpiibx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3mfnhnhfb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bknohzio.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wjheaqzz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3yhhmllgr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lbfrljwz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vnbrenhp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gudlzkxv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pymjlegg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fiskigpb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dspsggue.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hkszxjtf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3iqhmgorh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ijrelfzb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rhnkboiv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kmwiwuyg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qhdxizfe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3amnchlnw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3havwngmg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jqdmzdmt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3djtbxndh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwarmoyo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xnxllqxd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wfhftvhc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3llinlopm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cdqzywou.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lgasayxz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3emfxnzls.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvgzfgwf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3netspmsy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3scdnowlv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qlfjxvei.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bzctoets.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wmqjrmhe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ayidxblt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ljbmghmj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qcdojign.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ikvatoqe.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vomdjpym.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rjibpano.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3qwsepvha.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3iuvsdtvi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pneksvdg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gyqhiuyg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pzqbixuo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kfhububp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fdcyhupn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gzvchzyx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3djvvmuyw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3htafdkhw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lvlaiajq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lerdncag.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qmxrwxyi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kowpeylt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tnpobftu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gupyeggh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3aabyaeck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whkjcaau.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3twstwkvh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jwxqakvs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jflmajtv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xzoolkyl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3puddomvs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xmpfuyxx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3bsqjnomv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jujeukdb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3atycntbq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ddsrrima.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nrvznbcv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3axvxmmxk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ycgqqjcw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3rpugfzph.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xtogiimh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mekoduju.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zeebvwjk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jmgjmppf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxdooomp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3febfyqzt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vnwgjzod.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3adaswmvo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gifnychy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hlkbrldv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jtyfqbgz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zhlovfdt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zeeitsar.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nrdsalhs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3irdxluvv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ehtpcffl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nordgpoy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3owidjcpl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3probroid.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tjosfwdt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ccqmvhes.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jqalfkls.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vixfjonc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ewcbuazm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ocjfurkq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uauswulv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cimwshsy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3antsotfy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xhtqehcy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vtlzstve.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3gsvvvmlb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3owaujnpb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3rwvitmeh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ebkkjesz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wbionbas.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3sbjyewvt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rzoudilb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kmkmwvtm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3uiubliqq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ruyktkvx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3onxadpvv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xynwdmno.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3itczaxbd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tayyxkah.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3hoxojvdk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mlvfpbrd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mnmbzczd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ovhdpzow.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mrudxpcy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3cpdwxdal.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3muaimdqp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kjjijavn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gvwetrtv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ryrcyhws.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zpiqsgtk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jmzastjw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnupuqij.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gozdtumv.html


<!-- 参考信息 -->