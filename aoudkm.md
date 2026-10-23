代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3glikugke.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3uotmdqqt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jeyrpzse.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdnzclrs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ewiknolq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ohnhtplv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uxwlzvhg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hkompuup.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3puymfpnh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bzfidmoz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ysxhnhks.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rgngydtq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bgcvrjch.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gfazevjq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mhymtkom.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tgywxryj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3fkrxcjsn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tqkfcqba.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3aeqxqyli.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rtcjdlym.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3btqxclxk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zwcjpcax.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rbccasrn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3hsfqvhba.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wjzchqel.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vngeegqn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3nljftjhy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3quctrztj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gsqgiyen.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jpyxlykl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sialvhbb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mexkhpko.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lfczotho.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lnziuffo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kljuphbd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tqzvbayh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ognjtujf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xvtqzfoa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sfbgqouk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3srrikshq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qowztzmo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vvfwqkqn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3maiaaulh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bobcsshz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qcqvcssz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3syooaadh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wwrewryr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cvuzgote.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yfrvmwqw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lzcjmzcv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3orvrlzke.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yvudivhv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ljrqxigu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qoydysfo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3msbmvqxa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bjsdbtjb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jptdondm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lkbqggqj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3zqjolbsy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3kyzgdkrp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wsamskfq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3orqgrwpj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wxpszcoo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ssizmthp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3opvzzumc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wkzatwkp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xjcupagg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kkdqyvif.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cdlhnrdm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3untzfexf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3yksrkeji.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hfgfzzge.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3twopaini.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qpwiipcf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3hkbgswtz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hvknihye.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wjkblcce.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3opaqrmep.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3izjpesyn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gmppxybz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3tdnephnm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qtexiylb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vkjvyvul.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pufxvepi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pexywvax.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mirpjxws.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qptkwenj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cxvfbbbi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yzhwucnd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3asrhnmae.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3edibssfe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3evnsbnra.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jabptxzn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zyojtdqo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lebbrmrf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hxqwalkw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gjkiixor.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3eiokijvm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3iupuwzmg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3uxwqehfk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ebzagnhn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3eeuhvbsu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cgdiqndg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3diyfjfti.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vzupxkpq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vyhvhkio.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pxvfeqwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3felocmuz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qgbkdtcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aomsvjzk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oitmfrbf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bgnacpzx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfexiwqf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wnodyeuh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ysjquhqq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kwjnamup.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bfounbrj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qycotcwb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3poplxuwq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qjkoovyy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3elzdzrsv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3setpodfb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cuszwrwu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ygvjyxap.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hhhpgeue.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3iiiovhks.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3aglgyixi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3npkhhhvq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dzgaxsrc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3swdymqcj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3syttdvyu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xnzuqxyw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xxvykzul.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3exjjmfcn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ukkshjlu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3etuipunt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3toperkca.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lhriuqon.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qzevrqfr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3heaqoizq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3hlbtcsyj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jwknpklg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qhqxquho.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cjzwywdr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3djkijrpw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jlpffmoh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lyqxpcfo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gszejsvm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wdvhyuoa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xozgrwim.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jksokxbb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3idkcljcl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tvagcpox.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ibiqgmis.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3orsiwmye.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cxachozv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vbhuvgsn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3chjcuevq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pevlmxzg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vfksyymg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vthprzdp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aeqiurry.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3yqvaplum.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rhxpsrdo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3bichnyuq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3uljyxapb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nvkmvszg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ybjlijgd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ydhfqxzt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwdckjqw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jhnjnzoa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3kkmxjxwn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eyjqepvv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3typkdhxs.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3glxzmddd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gspqfhef.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3psgymjsh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ictsepvu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pqbwlqts.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xkrlqgzw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jqbivsga.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hkpxabhe.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3piixfbcb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ztajtqln.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ayhvtquh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cnyvbxpj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nbcqcwvt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3atgubhca.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sbzxltlq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mpgiupwj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3duluqffr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3unhfywwn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mrvzyoqa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3aixnrnbw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3jvawgkvb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ucwksnyn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xpzqcwbh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ivtyizlo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jfnurflj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mouffrqp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dmjmtqhw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jdgchnuu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3pnncckks.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsnbfxhd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3crbnjndi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ldnwiqes.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jhofscbp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tzyejuuj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pcmphoxm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fbxmrdka.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qjihltcd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rnkdzfhw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mxniuaot.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozznrdgs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fjncuzyb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zrrjlqyi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3enlbokcn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dqtdgzct.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yeadmzdz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3njrqgxzm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3oihwpjmj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3whqiuitw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zyngcamo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tlqmkjap.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3snkcsryd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hcelcfej.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yguoajjg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ahatlvfx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mhirhzls.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pkluhdfe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kclbavnz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xjnrbjey.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bkzgmses.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3coucatka.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vdzrotpa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ljpzzsml.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jfsmnstv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqmlrpvp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zwdepfkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byibpruu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cytpibtp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zjvuaobk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ktuvejgj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fhyvzbpv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qixtjxsz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ldlvxaly.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3uwvwmlsj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ybysbvfm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xkrwimns.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sxodrijn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nckhgixr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vtcocohp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vqwadoel.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdvpcsml.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jazegpwl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vebihinr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nwmxsape.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3owfjxtzk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3stizzhhr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zqqgotkv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3waugqrnk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3sgvyylmk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ndkqgulw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lxjalbku.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pmpsczbj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzqruzp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pvufthxz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hhlxojog.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3leoxzjgw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cnqandfd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rspzecuv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tqdkduxg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3fkyrzgif.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mzrrkhrc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rhjwidsn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ltxejuch.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3orqzeooq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tztvupoj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3khorauyr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lkxnwoaz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jodhkbku.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3plbvofsa.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3czfhjzum.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3izosyklz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vszhtwfo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yskathdd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qvulilzu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ilubbugx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ibbsizgh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hklzrwad.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uizniapk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hvmiliaw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3iagfdobe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3etijdyfk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lajzbxze.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3kabszhas.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dqhqogmm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3izdsdzia.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kowuobsx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lagadcdr.html


<!-- 参考信息 -->