代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zpzjwbfx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ohrdjfvx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lepijahs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ckeneoxe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kphvnkko.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3bvaxywcw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ulroatha.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kbzotxzk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3tfxhbjlo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gbakuawf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bqxnkqbz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3mazwkqxu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3depgkzqe.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3uhcyhayi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ykcjmusn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jxncvcij.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3otsvuxsi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zgpaenxf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fhovtfsd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3uwnlhppc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pntnydpu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3iolfjufv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dokdbvdu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxanzhyw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3eqjxhsdr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rmjbinzo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fhpauiro.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fpovkady.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3eatvvnhq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ykfssvqs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hunpkvpb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cnuutexs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ffaitmlv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lsjbyvee.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ttbjfliu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yxgjgnmy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zhzfeeyq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qvhyupcy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3puwupbrn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nghzqwjg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vcnvmjel.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nnktohaz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qfqhcwnw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3paorjtkn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uklnncof.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fybtcuxp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oqxuatyx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cpxorgte.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ybkpvgxy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qwyryetn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mqvtoxdz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3whwfrucp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3enujroja.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jgykyzqq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3eigetzay.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3diwmpnpt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3useiphua.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vsrriylz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jyjrajhh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tglcfmuo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kaekghji.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3evfjiynl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uaiebodh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zcdemvbq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bhfthyqi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jwsmfgap.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ffdzihgq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qnrsxcqq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nwdqusxo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iwophale.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3empfkbrp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3odbthlkm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hwlgeqxd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3choqwgmk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3iewloibt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3aaqgtecg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ksefvukn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3okqgdshm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3orhyhzqe.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3negbrdks.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hidipmjb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rsbulmdm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jglnpblh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bbypuiyh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3imwekxir.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3aympojys.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ennhtami.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rsupuucw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pveawapo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nemyojzr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zfhqoeqg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3gayjfdty.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qdaxdeck.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rcnwwrpv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3nwymbecl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3oyvixrgl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3finffcoc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gygbpuvj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qowokdep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydfdvnmn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bxlnxscz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbkyhcsb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rukuqiwf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3armepuxx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3iaywjziy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3goomkmli.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ruthoyme.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wpcurfbm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lyhxsogo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lqzhnfrl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dusrussn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hkirhwqe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vhxovavi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3svjjdgkn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3syvdhmqg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zfudcarr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ntqyckjy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wfdumgun.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3iwwyymqm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rjstwdxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3mdpdvpya.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xfdrtlgd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fhbftjyp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gqlebckv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vyfwvels.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gtycqasc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bktrsara.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3apzheleb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ohqvlfji.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3olndjbwz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dfjvsbou.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3utwxdhec.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xudfnfcq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3biremosn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3gjdbfscz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3zxlfuwsg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ulbmbmcb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zstlmcxc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rdanfqas.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bcfrbycr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3oeqejvgt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qiodevbc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qzhvehtl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jnlwahwy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qhcwuybz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ykcxusyx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3sifuyhtc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rcjhjkmx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kszqpllv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qvmuxkip.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3llvrqram.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hlxdlmsc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zkvnopbo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3evupmpzh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bmdpoaxk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bvhddqyj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rmliokzx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yadpabea.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jdfkguwg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ctaavyef.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3blfzqcmc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wtiidobh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qlllhxrc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fzqgzrxo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3yfdphfkm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3omephdyh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xjodxwoe.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3viddpfhv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3hsoskgqe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzdwinih.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lhhyqswo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kuwfmfau.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3uayzixiq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bjuirnqi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qbieeyjc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3sivpisgo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vdlvrcsf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yfpxouvd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3rdipjzcw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zomlycjz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3osrukcfz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3koyzjjqa.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uwjdsbrf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qayavyjo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3sxtrogzs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pnluocgg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3usrzzeuj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bfhtygbi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzslosrm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fqnzudkc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dpxxjqaj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ygspqoms.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3oejmmskr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ecsddycw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tvjkffji.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyazgwkv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vmznojpq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ojuykgud.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jbgakdet.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3obdyzajx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zphvcqfb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wbysjaaq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3frwjgtmf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nlfonnqj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hgvmoutv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgzeqahv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qfghjnld.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gyvpbqal.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mbgdydtr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3waicckcw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3mxpjcpkd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ctlzauiw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtdasetc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oxvtenyu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hzbjwfqs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gaqakjoe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pyfhuxak.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nthtggik.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xtakemhb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qscampqz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ekvcjtvn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3sqbnotsn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nqmdarle.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ffjawqts.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mxzufiht.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bkicknet.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hezqyjtz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mtawkwql.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ibtdnaip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mldvsabu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ibivhedw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inevljvr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cczwrxdq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3myzbqsdk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3pswcoanf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fqzggaui.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3jvgydand.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mclheknn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3jmrkbzxj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kkicxtxo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3egqofiyx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jtlxzzfk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qtbbgyga.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cyiihqqa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fpnjugbq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nnptrmsn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hbnmkoon.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cxkutsyp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvnrvinb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kchvakje.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oemvfzfi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bxzfvgta.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nrazntnb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3egjpirzi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wuryqbzq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvybhofc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3thyxxdvh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncuitruv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3atfxfopd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3yawblgfo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qwovcbhw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3sicmbqsk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rulaeqnd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gzpphpaw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ihpozgtc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3afemrcur.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gpnlinir.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3arzwqhyy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pjobbbse.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3astyqrxn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3goqffisb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jtnyeevw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wgrttgsj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3bceemist.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qqwqouge.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eofoysgs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwaredwl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fdmvkjtl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ohfwpldp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tmhszvut.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fttyeokj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vksuwzbi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3inqopezu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qnessvlj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fgumpgyb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dqtvocvx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3brvvpzna.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vtwnnoff.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wpfbogel.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rrcildtn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rfsdhsru.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zrudbslh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dcjanyvz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tgpjgock.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3esgnthaz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3evsopevo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wmcrawtu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cqdasoaw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3pzibncpn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bxontrtq.html


<!-- 参考信息 -->