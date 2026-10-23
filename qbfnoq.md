代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rtewdnjk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3oqulcczw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbqfgyrw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3skzfnqkj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3djaywqmz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3optfudqb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zllmisjr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bfkodmrk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eavqgxun.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gffcpxtc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qekdbhux.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fjhgkktb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uyryczzr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bvbvjyfo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pvybosuc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3isbudytk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wofyquol.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mcduaxlt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3uhjcahoy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3guawxtdo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qiebmgqt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bicftdul.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ngtktcmg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3olsyuybm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3dokmidtr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jplvnvsw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jppijnxh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3eqnmdoom.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xpvgtuug.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qixsjbug.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3btyuavlz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3bbfznywu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ntrxlbco.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ccfuzfyy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3achfykac.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tkcwkqef.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qyzkhepo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3cbbiujtn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lydjvydb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ugtpuuxb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3skzprhqd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zqqlnjqp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3syimsphb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mmxvlxkm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cpexvdny.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3axginguh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gddsqmyu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vhqsqjij.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kmdzqpzo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ajoyqeom.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3uguosuvl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ocqlpowc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3unftmuvv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3odueoobv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hxdkzihg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gobvnwnl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rknvtnrv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iuqusmph.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rigphdxv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nvesxnyh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3riptcntx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3emqwouby.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3lwroyfkp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ujumuazu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jtpeqvrp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3aquatopi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lwtczaow.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fuoeagdq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lwprojzc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bubdsazz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hyamkcvh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3adancagc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jqukbkuz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rpkdngwy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3nlwxxubc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3uvvwduwi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3dicgnhjm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qjokvxlv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nqdpkqby.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3enrirbez.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dngvgsmj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hlwmybrc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bsicotbw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3glgrddgy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tqprlrdy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3tivgzjig.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xeoiazcf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bcsuomdl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ixsjgefu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3nteyqvde.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3roniyoqd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3svsrvcme.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vgkcmhxo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3tychfxrd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bywjwgqf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mflvljrp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zpcixwod.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yegjzbod.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pufcefqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcuivcon.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3bmhoxjwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyshadkg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3udvlxfud.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3uhjpvvln.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zelwazyz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jpiurezb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pihhveen.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bftgjyuh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3avvquzff.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xspasqbd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3thjmuvti.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pzzdbyhf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvebhngm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vvwknkbk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3shfbkcqu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3apkscdgn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dlhwthrp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3umfhwube.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ennyescn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ixhuvmco.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3fhibwjer.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wbqossot.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zjnerodb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iamtgxge.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qkexdngh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3djuswqdq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qyxehksa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pmtfdeec.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lxpyvbys.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jjgziavt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rmivcacj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3agrouatk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3pzhregzq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3auqafjlf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3vjayoofd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3thswpeem.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tlyuwnju.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fljpkdlm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hztvuiyj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eoocylco.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3sspczunb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qftedbtn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3otprogsf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xmwzwyjv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cujhnrgh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3alfmocos.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dnpxqgca.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yxbgrpxg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3znrttlch.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3efhuzbfw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mwkqmqmc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zojxajuk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qeybalce.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3peybgmsf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3mpanfngz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yftidtck.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3raumvnin.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xvabxpfw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tgosorqz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gzcyuwjg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cbgpjltr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mgjjikgg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ktbrxdsl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mlflteer.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3onkpojyb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hnfhprzb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3sfahhkxw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gzvaufxk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jyjnaiug.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxkmzdke.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jftmxctp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mxikzuzd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ckieiwjv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xdrvksdf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bbfltjnc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jabhowfu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zzkfoave.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fbzpqjrp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3yvirxuhc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mpkzyrfc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ljohajlv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3stanwcpd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hsqmbfkw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yjvitbsy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3skfyzhzd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jaddwbho.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ffbilgqa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zojyzkfq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlpxbrap.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ypxrqenk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3fsdmahwo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dtolzwiu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tsunwhwv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cuerkquq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hocwdutv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3anlpmlew.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mdxewzek.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3pdlkplvt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vqbbqcjd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nzjyvttc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hvltlchl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kvesccjr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzchbitq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3iqvwtvlx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ogntqfdt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3oazjvpxy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mkxkngju.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kftobkrc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3twgctnro.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mujyblaf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3mxxbehhi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3angmxpbc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3djgcrisb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3asndagew.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3slnsxqtn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kkkaydpc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3cycwnvky.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cowasqgq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vbhkzcor.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3oyzchynl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwyizpeb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3drkhafkl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vphrndlt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mrecnazx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vhmtwbcn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wfyqmazi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3chffqvob.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3abwbcxxd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kladlnsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaexjyyy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ukggmiuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dciutyut.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tvfdqkby.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uykfjbwt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nlpalfav.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lubaqzzd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jgbvvnfb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kpshrflj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mhonudcd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ndfkbtxl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bowkmhlz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ooqjlnjx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qowktrhi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3relymnzy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pnlrlmaa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3udwhwnsn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pavoqnmk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pqoxdrui.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3pdgduciy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jxwmlchm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hqyggyle.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3yinuphtv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cglablsx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ijqqldsl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3egbfbsad.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jkrcwgtl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ubhgwyts.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vwiejxfa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yuokycqw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cdzvmooy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mvsggzxu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kxntqwwk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ihhnfmpd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yrogfzgn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3iqjntkzy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uqixjmly.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yyrqiuto.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zltycqjw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ldabmfup.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dinnsnjj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3gggoftuv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhmxxzm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rjagpshn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3nrqwjpvn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rzyyhder.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wuykzaaz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3amtfkili.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hcnjcyfc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mudqzvrn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lhtwehwc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3rjkilbbu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ikvabdwl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3slaqwlaf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3saygwozr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rvgqdelp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cqvqwxzt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3okaxojvq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rclmauwj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3yzjjbqld.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3logtgyfw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zpfznfyt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yenvzetv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zafssfdt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tzdqkkpm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3eyiqwozm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rvjeugqy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3anmqdyvy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3tffvnugr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rkoxwdnr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3qlmigpmb.html


<!-- 参考信息 -->