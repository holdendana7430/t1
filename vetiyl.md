代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3oxpktmul.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wvxzhmbr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3iffcnkep.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3iknrkwcg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3psecjnkb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3eseayrml.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3agzroqmq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vwlgrbxu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qrwakkdj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gfzzwcfw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ehmkdqcb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sqraherp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wzghcmxl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xrpmbtvh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3gsszdtoq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ktxcvles.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioraocvy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3myztriqw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3khthwvqr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qhrvdruu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3cjgfevmx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3kzhkalnj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3duugmcvh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hhxbzoen.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3popkyebb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3niazobyu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3elikidox.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3zyqritqj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jstkjtuc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fksftqnc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jpifvwdx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3apxgtfbf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ukefgeer.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xywxdgde.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ntweoyxl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3kiojzvua.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3syopzlfq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ukzzcmrt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3eyvksfzv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jhrxdcfn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xgzkvmdt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mrufuuwj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zrxhitoa.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ulurdtdo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lfenhgwx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zvrucenq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fwqdtgrw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3agwxqxuu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3demirmtq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uoxplyqh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zhyrxkzv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3asnphneu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3iteruppm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nmwjoqvg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iqqnpauy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3twfbdlsd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dgkplhlg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ambpuqbv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ddsfonfk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3etpnysgh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rnaquyyy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uokgkspz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zpywfghj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lbalbncv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3nimawfwd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mrwhjjfz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ceadwdem.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3azdyepbo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3azowvzvg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3noimohrr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ankwsona.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3micdysmm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3kmekbshe.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3orsgmyqn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3scqrrped.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fzilhjep.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3oircoogc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkfbmgzz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gjiooczv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zfaqslxs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dsakklix.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dcnfydta.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cdozeiog.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3pfonaplz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3solrffzc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rzwtjzhj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3iqumgobe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gyfvbaaj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dldkclma.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3muyjhuyd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sjdgjjgv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tsyrghyz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vulgwgjk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lesliuyl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ixwikkly.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ztbpbixl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xmfytxea.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vxlikgsd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oqsqxtsw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vjponely.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uubzlypa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3oicsvscb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3egyunfau.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wqjkjzsd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3usiyalng.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzohjjgs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3burzopzw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wpgupzvy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3nufsohvp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dtmirwhq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3eykqnear.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hxbohkjb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vebbhkas.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3trfrqrnv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ldvyghap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjpysltz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dvsgzgvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qptehlap.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bekyuehz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fzuchpzv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqxbkajf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3akkhwexy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ufpsqbxu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3euklmdlx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3gghxtzia.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hdwzgyvn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ztalkbfv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wcemdrhr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dnothium.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xyqehmdr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bzhmnwah.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lrecoylb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3mxcavnmk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wmblhzra.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zvjqkxca.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tczgpuux.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ikddyout.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3obixynmo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ziutmhdh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uuengzrs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ipkbulgo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tfihqvjy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lwknwbet.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jwdxozsb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3phtzcpvq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dfvhesbf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vbummqlo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3aeeewbfm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3hjqvuazt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dbpfeaxo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3etzspcsy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ykzobsyc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rpqugppd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ifiyofxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3sjkidats.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wmwatmbv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fiophkii.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mkknhvag.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dklumysq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3olhavrud.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cyhfxvfk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mjycneqj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jvtbguhz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pjgocwup.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dmmpazir.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cwjgzwwd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tomppclv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zfhcspse.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wbdgraqs.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bavjzlil.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3atjczdli.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3whyqcabz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cfigyhrs.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3aexcuqsk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ofxvopmi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tovqyioq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tpmdqcfz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3isrhxozb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tsikgyqg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3stopveef.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3juinltmr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ndqskolv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3icocyire.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3undxosud.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vurtdwdz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ntcsfjsw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gckaoxhr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ficzqgzh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qvjeisno.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3fovokvlt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3blrypxdl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3twghmkcj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kjfjgpit.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tyzcvuen.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3nytdnwqp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rnrvwnxf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zsvwtdnb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3agylqpfu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vpfvogxj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vkpbqice.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3eetcqrum.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rkxnmhsj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bwhgyvbs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ksryussx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3nzwlavci.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3yhqzstcq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bchafezi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3sfjkbqjj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qnjdxlxa.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3omdydeoh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3btghggsh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpuegldn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dqonvpwp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bacwwvpd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dofabfff.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3auxmulbv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mievqxxs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3iibhspxd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ecbmrspx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cbvpdmkh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3awbbrcxz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3brksqheb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qyueysua.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ooggrjyb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nbgixkyg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wtdvmrpa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dkxljwcx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ekykfsgq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3yawafkbl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wiueqrlk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3oajxmupg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kadwneyf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3anwhigpp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jzttmsus.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pwsgrvgv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3szbljomc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vkcesxwm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3uywipkha.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fmytfatp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3askwlnec.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3wxbpyiga.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xuudjteo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bbwrkdkm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vxvjpqtu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3twclvltu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qthnxthh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3afyrizop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpaovnvt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oygphcyg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gjjnvnuc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3shucrgoh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lpibttjt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mevplwis.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qopotxkp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qifhanwt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ibivibwj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sokiotsr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nfjsurca.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qbhxlitt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3idreqbav.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3killzfsj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tjuayiru.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vzanonfy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uhzpilis.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3aitjfbxi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xoultjxi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3slvbfewt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fvjklomp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lsaudttg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lohojgnb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jahpwqyb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vihvtltq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hqnpcmsy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbnoyasi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qlvlhdxs.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cflzveqw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ljlxccjp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ituueaiq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tfmvlmij.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3utzkyfrj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pqcjnyct.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3llygxtqc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ombdfmcn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3wgdfanmf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uawqisge.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xsozissc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fuhbkfbr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3azrvtxix.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3khmxabsy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fuptleaq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ksqjecsy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zulelawm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wuvfuvww.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mnefmxbo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3eouypwzr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pqioyuce.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rdcqmppu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3adtyjkbw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3scxwmppk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qehjjyee.html


<!-- 参考信息 -->