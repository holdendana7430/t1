代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zfythcox.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wyzhahei.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gxpqysyu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3igmhibbm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mbolcnea.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qmqyukjd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3eerrzxir.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nvtyiypp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxcnvxic.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3elmbdduo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pznudcol.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xegrnanw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gkygphvm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3slzfmwak.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dcvvfhtn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vxsjcigh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vlvbhtyp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wklzfygw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hycaeprx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsfoyylo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3adglherv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3wryumejf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3yjdjsmff.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3aokidkjq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wvfmkzzb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ytisptga.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3qxddskhy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qmlalreu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ynvumycg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oumudmzx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kosoqkqg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3pbbvwzir.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rsinlqpr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wcuxoivj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ohvkurve.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bgncsuzf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wayejerd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fmjznzoq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zsrssjck.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nltkqqod.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eqpzvbxc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mlkvxvsv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3jbshkrtr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ptjhoaai.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3iuvniqun.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kiivtzjb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jfkiynpw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hompyquv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ebzadntv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkbqvfyw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ukppjupy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3firsbqil.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ajqpullb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3djaujtja.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3iodruziv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fycbulem.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nsvaerwe.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ftqerpgq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rdwuucfx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ufjeulsq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ladpmhhi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3cskujewo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cclvaajn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kzwhkshn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3revwlkpf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dyyqurqd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mhkdjhxp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qmulnxsy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tejhzcuz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ogrlkwox.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gfzpbtca.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3bnbktfzp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rkgqzswe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3twwbtsxf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ozkigity.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ldpmuvci.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3opyogvis.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ulqhqojp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vpyxldbl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3faltpujf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rwnxujht.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qhzscjyi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3exgqracn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3blsqjaip.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ujdjwqut.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3inefhgrx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zxgrohla.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gcrxyzfm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3lvweacnb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3iejxzidi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nqnvwsne.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kqvdupyp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xrafuidt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gsjucomm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mckchlvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xevaksog.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3uvrplzlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxvckhok.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qhaimfkk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3brsjivwd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kkpvvcvr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zvetejpz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jyuzzbea.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nzobpejm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3apybmqpv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mpmtilpt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hazbhhwy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oashrtsf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3spxkkejv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lpmsydim.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bwlrwlki.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ristaizc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ywpzdpas.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3aulbwoqa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3abuozvhq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3szofqafg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3dtrdjgmn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3chsiiawc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kigfwrrn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wfhzexwm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3frythnlg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3symmgdfq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tknwoeyh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pxzryqdn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ewqgkvoj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3usjscczw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cthdpxof.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sniuggfy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dwizkmlh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tgzfsbln.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wlnabbll.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3teewkhiw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cppechio.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zcpjiwdo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3setoryow.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltmrsacj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3csfikvdy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ynzjrzia.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3knwwnefc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hqewtxnv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wzheledk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cutuusnx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3etfmyanl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yikwafyh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nryfdadp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xgwobizd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nniysmxg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3atedmzai.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ogynkabh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dudqvkxi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3krebeqnu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3dsdqpndo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3iqygkynb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rlmmsjmp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ktlfgmai.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cqnwydme.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nbcozgie.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qmepjayc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zavtaatp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3higxtolg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jlczoxoz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sqpshefl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bkjfrazi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3osaqmcty.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3plekinog.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xexietvq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3chikwfeb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3cqbpeozs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3yuvebypb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dulyvkzb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kgkrricr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3clrgenlp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3swffncin.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mixiyhna.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qnxskscn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rmrdhxbg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cctoaeez.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ipvsrbvs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3sihyxosi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dhtfhnmw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3txhxvtmt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3uaiktfru.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qaemkhvk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xdfoyhph.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqckhyzh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3igwvgvqt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sobchyft.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tttneotq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ogchfddd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zddkcngv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3euoejrkm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdrwgjxu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3fxoyvtgg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hysmqwtn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wgmmpeyq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jkkwaden.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hcldjklr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3evlwfdun.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kdwobmhe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hixezmno.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxcnvsb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bqmccabg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3sqtshizg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3coyczclj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3whxniodg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sljlwujk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3nbjuptav.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3issnobkv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahidwwne.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3raqtpxva.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jdsxtqjl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3yzswcten.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fxtvcohk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3adkhdkmb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aciqpfne.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3sabxqltw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3opxeiali.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3sdtqubtn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tuhzmuyh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bxcostsn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3grtyyhoq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rreoqlag.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mmwferjf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wvobdccw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ujnonxbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhyigmma.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bmhccgay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggqzauae.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ahopiqrc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rlnvyevp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zqujzoii.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vrmvodvg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pywfpgqm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sudoimyb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hiipnwie.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfmhxlzv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nfqgcwvm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ylsuekck.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zqgtggsl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kcwjdycr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rbitpxuu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mfypkrxz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qqscjhuy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rnociryl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvoxhlus.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3apfpxukg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3shxzsuqa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ciybpens.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qtvnfcwa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xxhqqqoz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rplmpukx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xqibwkqk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3anfqfltz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ophadzbi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sbjpjddq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rrnuvrvi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xcaiqsla.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pdznypgx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bmjctykb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vwtcdlcn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yamzusar.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jgtfuwaa.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zzaikowi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zxuviapm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ewmvwfiw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hzikgvah.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fwfpjmla.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bfcmujmu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ecmpzjtv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dsxzputd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gyliyciv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3iuktldao.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjuhoufo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ftsbifxe.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hkiqslbi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nllkortl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3odvviiyi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3yzglwohs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3bptmbnlc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zfdwqkfm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bhsxmuly.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ynydtcjs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jfszzegs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hwnlvltb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3teitfhzw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3uqyijnsk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vgitmnvw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jpwcwlod.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uxwjyjqb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jpfereld.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dusuynhm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bgypqrbk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nfyxkcth.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3yaooblqx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ojtmzywz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vrhjgjwx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tywmitki.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vhzwekvw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ymxbwryi.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ptxgajuz.html


<!-- 参考信息 -->