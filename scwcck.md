代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nmlurlsi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dyyhxviw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3immdwzfz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ukfnhdcg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3htfzorzp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ooohucfp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3qrxjilby.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tzhuyorj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hymoedjc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bjbwakgw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hidpzatr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zkrycaam.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3enzjbvwp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xcgbmipm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jnyeewxo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lkoqvwcv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qlpoavfp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qbquwsco.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uxtdophe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gzelhunj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uiopburw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3eqkvzgaf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wgzwhkkb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fhjkapxa.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xgpcspud.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mpxmgxdy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fnlepnof.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ckrkwbfx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3scylqaqi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yiodmkkf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ynwnhhch.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qjstzzmu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nlajpzub.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tiistmrt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kvtdrzvv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ahlgfbeh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vtvhlwan.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ibjyxofu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vwdmqsek.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hrwxyysp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zbvrujdb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gdsixper.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vvjjhajk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rktgwcoe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3lcdmrctl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hbmcxwmi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mpudsjvk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zaazlyjy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bxqjehoj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3oamhvocz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3keeplhbe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3voubvmkh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3veoxawpu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iasfxzos.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3tjjhzjlb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ndjspxyi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3frsdpcwj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3dmgchoki.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zomrtalb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hnackhii.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fdwetstv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3uzdsmanl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3azfdcfbx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jbyprjkd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hhjoesbx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qvswsfls.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xwktrysy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xrahammj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3bdykpoll.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3madkpvlm.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3anlpmzbs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3forfufzm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3lhsazbrs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rotozmcg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xaeywxvq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3teeepnxa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tfyodgyr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3tnkkckna.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wtsamtwr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nficrtap.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3uapujpfb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bywkvkzl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mlistbkw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lkuimopl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3joooleli.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zpqygcsq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kicwvrqd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3trzaljuo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ulcsmysf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fuauorku.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vnikxldu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3crsosxju.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zrrxxdrp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rjhjskvz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qhyliwon.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fzsgyozi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3eeteltkf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvgcyxej.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wjqnwarv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3chvgiqgx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3sbdctlcj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dydgmjpn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vhrkepjb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ojuzkbeu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uosoyrva.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wexpejbr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yitryvna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smwpamuf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ksorrvdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eodrdqdc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sqlerpbl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ecimsbtd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3iihagyzo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nokxepnm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3drytaiqo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nkhsxnot.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ruegdwvk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qjegapfp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oucsiunr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eoambjbw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jciukcmt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjujczot.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dizhjfrk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jxmjwpdn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3eqlscmud.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ptzghhrk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3wxqezilt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ulhtckko.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hmuxxhng.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rpmamduw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lolbjftn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3llvzcsbl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nshirbjm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tocbyfvg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cueqqjtn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ycbkqbvi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pheugwry.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jrvkenli.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3sqiaggnr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vltczcyv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3htfkdjwq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3goacahqd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3knlvgokg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3itsonirw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yofrhgen.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zzaizffa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wdiilphi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3snumyzvf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dpogbzjl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3eamccbek.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lpmknsgz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rodcazqg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ncolsclz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vqtyzalb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wdnaxhpv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uurlggcd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3eqkkbavq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gcvsnzoj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uuksnirw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3aktlieqa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lqqdbokn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ygrmrhhs.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cqslflhh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ezbqzcul.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gkcvbxcs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hshoekxm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vtfqawlu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ztdrterl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bcugojxr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vbfujiyg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3hcgmlicd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pkyfwlvz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ekvhkxol.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wrnfgqjo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3pkqsktmn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pdlyjzwb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bchofahm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iavegibe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wnmdylrc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wgjtpyvq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tlcgfufn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wxogoivf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mbfmhxhi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pqsoanyh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ftafbcro.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vmtqbwkr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dncganes.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3chlryjnu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3arekqrjs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3grcblpyf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rftvareq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vrywgseu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kkpheflb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hjkgsggc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ecftzfej.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mvdjdfiz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rahlhrjv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3crsbkxlb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bnnopfeg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3drazfzwb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3uldwbaaw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3osswwkdt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jrdnijtk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjuqsfzi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3juqfbgln.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3virkwsel.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xrtttacd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ixjuzpcq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yijdture.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3uycuwolz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbgtfdxp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rpyccavm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lkukzruy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmidztpn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3prvjzags.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kuqhlrvn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fomrbsqr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3khugwjem.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3onuzcmer.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3recosgol.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vufvqqoa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lahdztfz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3seudwdaw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jivvuisw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3djsyezhd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ndiqkinc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pisotgxp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3uraldqts.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hoqreqwp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jnmncmfr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kqzxmgfj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ubbfdtqx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3avsgyvvo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kojdksbc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3taguqjpe.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3meednhbc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3egjcioow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nizxqpls.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lnxqcpnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cchgznhq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wqfwyosf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lsxoktbw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ucdldqsg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ffjjbsde.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mubyrfcu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uysveuii.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ltxfvtes.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zrszarnq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vciqadln.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eynvqkhe.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ycqffwui.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3agolqmlg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3duqreqca.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mlimtlev.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wykakbeo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hwphqvgt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zwjbmrnj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qvoctumq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3oqpyeifw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3nevedfti.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wzzzknza.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3aklieacc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fuaunxgl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvcympkc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3eqyjpgis.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjeocyvt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ehohzoes.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ippzjbny.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3dabswglq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3peitprqs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pshctgmv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ueilhkwv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mmldronx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zucyaapg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kfnwukrm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yaqcrvtq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gcdwgaay.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3wkzedbwf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rvqiabqc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fmqjpbuv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qcgqlagd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xhevemyv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3cogxjwxe.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xeuiftvt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wlmtdvxj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gxweyipj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vcibgqkn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fozchtmf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ihwmxfic.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gzhsvjyz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3boukqfvv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ixdayzqk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mgkikmvy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hjaqrldi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jlayfnnl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3doxzfxbg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oicmlvxa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cfpchffq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3llcdejnx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pkxmeldb.html


<!-- 参考信息 -->