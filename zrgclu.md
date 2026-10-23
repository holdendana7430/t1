代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ondwhvxr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ibwnoirt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hugypyre.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3muaypmhg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3dgrdwvnb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hddmgzvj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3iraglcyu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mywqvzjd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zbqmkkym.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xdfxbnxw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3nzfdhbmz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mtkhwxur.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ewmowabc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3deiswnqf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nsifvcds.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3oltxscmz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vvhegfrz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nbxhcpxc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3oxszgfxs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3usvkoofo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xrnqssjl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lhlunkve.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3uwvuzirj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3agmhmvat.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lraysraf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3draweqsb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3znqgtier.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qtvbxvru.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wmdceata.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3aydfiklq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ssbxpnfs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hyoxthvr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eokbkzak.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jhfmmkjl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dbbwiidg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3illsvxig.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nmybwcmu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cehttgjm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3macrmmpg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3aoegetez.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dbpmyfak.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yokeorhw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3lhepozrv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3cylpoxgy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3oagamoki.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkxynwxi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3umhvuprv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3urlawvjq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3huzxenrb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3eabuohxg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ydyfxqlt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qxbmbkou.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3msqopddl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jawixaqm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3pilgcibw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qvyzuydq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3skqwuewl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tlnmfkvf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jqiubglv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3sccndcur.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3bbpinccp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3aslhdgte.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xfkgbvpc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3djcmuynh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3obktugqr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mrxxccxz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tzphobyt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lnomycxv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3pfgvckyl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wsifpucl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3aqssmdqq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ermofltx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ojgpfxqk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qdmmelme.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jedwsqys.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ivipplvx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yvqbucyf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kxigizjf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pammxqpi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yjqdmvot.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3elwgylro.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tgqzwhdj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vsbkjpew.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mofnjipp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rlfgstdm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ohgmzspx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bhmbatth.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnjhluam.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ooxuhqsu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ctrskfif.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pekaxhnu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wijczzst.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fftasqes.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3kdvvvqag.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lulukuzl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3cnkydkli.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dyvilgzz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xbmpjzzv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vxlkpxce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irgpwuxf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hucdsnej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfzgoysp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tfmwwqxv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rbotntbf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndnepcig.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3drflohcw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xinqdnzw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ygfculmg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3bcueosum.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3asviobhe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3toysyxvh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3osbzycfu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cpjvyjwu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wrkpojta.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hpnwlqcn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xtciwbwg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3aovjuylj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3sprmmpfw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3auoxgifw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3nlcltoce.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ohzsuahe.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lgyceptf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vtyanyru.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pyedixao.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yqqymhky.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3oqnaohke.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iqcvexwa.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqpqwvdi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nqhtkdoh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zrefkxsq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vgsoqtva.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dbpqtczx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kyhpqwxl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qoixnfse.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hcwuhccf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3kjczsffh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qtcgvmzb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vcxaofkm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zsnilkok.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3krscomhm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ijvhuvhu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qfjgmszt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ednitwxg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3holewidd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jqpdjnri.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3abunxvch.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3prgieokf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3odhyvldf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hzfkgtwm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vizsajnv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3czipvtzd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3didnetey.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3eakecyba.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3znosbrsh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ocfzvkxg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3oqmkooau.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vkjimphb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xebkvlgn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ffpxlvif.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3khgvvphy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ahsqtvrz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bfdzerwg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jbukgoxh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tmuhafto.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xmezywqj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ftfssqiy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tvaolfeh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ysvkodvm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yasltuit.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aclcqvnt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mawgqcfy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vwdptnln.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zpeiacnf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tzensgkw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jitzhtnh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3occxiscx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cyfhdzol.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hpbegrvg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uzpxyezz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rqjwsufw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dmhpgiig.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rlzlzujj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3uqgbzqwt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3axtimdph.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ymlgkkbg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vmoemzhb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3furvjwty.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wenwbbqh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bazcitej.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xanhjlwj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dwfnpzsk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mxiporgn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dlyvpurw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qyxoezcq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jgepfetx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jburhmly.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mgqzeuse.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bsglsqxh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dyqoqojr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ccxqxdtx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ieeclyju.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3eanwzdfa.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mfgwdwez.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nhfcahdo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mbexpqhc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jiqheuda.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3pqjgvhyq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gdprciao.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uijuudhs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hpykdayf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nbfytcql.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3uiobdlyt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjqtzqgl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jzpkwbjj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ldelsucp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rldmgpzv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3klevjtxw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cpqqokic.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jhkbewik.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vqptrgnu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmwzufrl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nsyrwjlc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ljniylco.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3cccguiil.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3szfqbjan.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jylelsdm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3efgtycow.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tblftstf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3eypxxomc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqalarwk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3oglfrpcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsroulaz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ivkqoavh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gezpcohx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wgveyilf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3npwlunbl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3seupbmtu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kwxcsquy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3zxcnmiqv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qnklbxrs.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3voysfcon.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rqekjtbv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wblahxoj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mjbniggk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3slkcmroi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3odnpmjzj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xxmyzitn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hifnjnch.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjutbskf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3koiajqij.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qyornnpo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3lfaygcwz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uilwcwyw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nehokosp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hlabzxdv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ishrzrlb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yqagfrlm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ouwohjey.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ekvegayd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbycgeg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vuazhbcm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jbjvtlrm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ajfkpfpk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cbhnwiqd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uduorrwv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3skhrcxjm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sappoemy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rxeguojw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3rtldedxd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vusvamyy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xthyngft.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3issdzemq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ppwipgzt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rgodrfhy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tiwpkzhp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fwjisebx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmwihydr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vhbiflqq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ezwatxwu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nwbibrgl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3aqsgzqfu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tghfzcht.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3eaistohv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ymrsuuym.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3uulszcjr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jbhulktn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ricusmzo.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bbfrbmqw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jxficxra.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gzvmtqeu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wniwmpqg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qwyndlrf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cpubawoa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qlcirgfh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dytiyfwp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mqblcaqy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nywxsimr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3dhytbzct.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3nmfuspyv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tdtfhcoj.html


<!-- 参考信息 -->