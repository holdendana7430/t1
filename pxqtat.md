代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3spcohcow.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3btxjderc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hjzvdghe.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3icbtwvjy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nyvogfjd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nllxdyjs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hcpbfwtb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xzlvauiq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ftbvfkri.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3loaawygg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wltfoufn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fngiuycv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hhvputtv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dikzybrh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rpakfora.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wbceivhw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yfajcraq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ekwjhhhe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hlucrjom.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wlumtsuw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hzjxmztq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3judooxpk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hedltfrf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zulaygrl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gamlujuc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3yghzmpju.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jbsczoqz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mwedhvjw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wdqmhhae.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gbsvopmi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ubevpbva.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3oogedgyy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3prqaajam.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tvbvxqde.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yyvygiyt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dlobyxwa.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pczoomzl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jlmopeep.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3bucgqpbu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ckgiadxh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3aokimeog.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3nqqylugc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fvdsekgs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vhxjonco.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rudjxhmb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3weklypew.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3omkkvamc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ekgzklcl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xzedtzue.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lmxawzxo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vuupoupb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3neyliatz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yrdqpkho.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3nwfonxkl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cpfaxpmg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3adgwsqja.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cocxypoo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3epzotpub.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ugpcxmmt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dszavzln.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3pggvrfeu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3eutybaes.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3orhslmkf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vvkgjxvp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3evbxuoyg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qoqayngb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3fkbzwayf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wibyjswv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ggglrdiu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hyziioix.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jzwqgtuj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rushsivp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3sieglgpn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3eorbjjhd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wtzyhffd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3csovivlk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rosdqhny.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3djylvbxs.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jlswawap.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tguhpoqc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3oqgujizl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ebbugjsa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3olvfbdba.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xqiqixjg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xilcgrsz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lvoeqpxl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ngmchtjt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xkcjgliu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rlrhpuye.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ykomoghv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gimlgvoo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rprqynlr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ovndecwq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hbhjxvkr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gitxpjas.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tcqphgce.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dppzigha.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3abhmznox.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gbvrkcwe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ohflvcgj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xrusrlrq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mwztovxa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mvzafpan.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rbldqghr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3irtdqlfd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mguctrvz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mqemxybv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3arkfslsa.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qliwxxgp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dsclqcnz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tidnoroh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ovstwngu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3rcggsozb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rchphcal.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uslqxmta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyxfvmdv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3duebrpsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjcchrmh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xfauphvh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3agwsidff.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ffggruco.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nclkrygs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3svigrstb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gdytgmks.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nfxzxtlm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3gpbcdnhx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3athhzxtd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sbipcyra.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qzjwgjar.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ehzorfdn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3tnccvbee.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ldlrrkct.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iitbmohw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eiueztgi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wewnzyzs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xtqozaut.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3yuwqlzoz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kxmlgwjw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hjgzknev.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzvhkcxj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3elhaeyue.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3atkctuog.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wurxlgoh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jovtloui.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kvtpwbxu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vidvqapo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3oxjernur.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3erhekalk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bdatnysd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qrakwank.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3algwffwe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yiuxgyiw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hlkztbza.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3megijtwu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bfufzwub.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yrjkrkhq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3exjzfagj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hebklbfb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3awtguwrd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cbuneevn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tmnmqbfo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nihowvjm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tkddgani.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fbcqkwhw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3cgdypobt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3umwdwfyp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hwhcanvi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rmjxprho.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dconbtco.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3aiqufzzw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pbvfpkhf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jyfcxaer.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3crzmjeyw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3govykspb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nebofqtu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dcmagvyy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3episclzi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxugqvhv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3nvvosvvm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3blhnjwar.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yrrodioh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3exvttpto.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zsbpueac.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rsnygffr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ebjcupiq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gagtepqj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fhkxasdc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fhzkyykl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qdolsger.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kwnzxrrq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dqnmlfjr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vytqqfva.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3isyivutc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cgwthnyl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vdojokoh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rwybfgeu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zxlnplvm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qixizimi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wuybtojk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wkoyzdrc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ucqqerkj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xlahtoiu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nnkzpqge.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3nodszjdp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtomekal.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wtqqglwq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3fiaofsjm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yhsiogoe.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jfvnoxpi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qqkgofby.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pxchjeit.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxatvdet.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qakifcao.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yiiufwhl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3negiaxbi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3elkeonxq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nwtjsgpf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qoqjqyai.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eliochpd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lhdyzkrf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ywrvhvez.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zszspkgw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3syjkoldt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3sugwmrkj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3migppcxv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jksxoent.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vxhaqbvr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3eylmepih.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fbudwoma.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xbinnmkt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ieduwaef.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pmgfckvq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ekbnvrmr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yvnebeel.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ynfawalm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lmiqronc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fumwivyv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qttewjsq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xxewicke.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vvspwszj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vcnlsouc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dyircysr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3plgfcbvc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wdrgbbgd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ulzamryy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywjtdilj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ltyoxnab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duvtzotz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cvjakpgi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rchyxmlz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mssnjszp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3aueovajs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3iriqudab.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fyrixmlm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3eunwrbsu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ejegfciz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ieqadrie.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3slhnhyag.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3esfoqwur.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mqydamnz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3exlgdwpx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bznethcb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vclbjwvi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fjicphel.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bxwylmpg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zxwafzii.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3mmigkjit.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hvvhdabf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3tbhtaurn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wlalbevz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yfnfeeev.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlddbcyp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kwygvlcf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tslupxhd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cuixdbrh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3adujewsz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rzvbrqnf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fhegvucr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ofggtkjr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3haikztxw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3yfjuhtki.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cjvejkvc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qadwveab.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zivjxnei.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hgegslew.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kwmsufjl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zmkfpdco.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3erwmhgoy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3azfrahaw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tpxoxhsc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rmppjemc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cqalnsii.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpmgpuqd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pezhupka.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lrtkbcab.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3maluappw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3xoocoobo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3krjvtiab.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ntmwsxdx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tyysdnxs.html


<!-- 参考信息 -->