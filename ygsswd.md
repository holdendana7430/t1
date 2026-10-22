代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qznljaze.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jaevvuko.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dpgeimyd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xvrglkbw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2unlqplqc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2uodviduo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pmdlrdvq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulssnirc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gccezupw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fnygtbsl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2awlrdmcv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2trjzotse.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sltnchjs.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kccfnlow.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hahrrowv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2awiicjzo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jwcdyxiy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2huatvunp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gbcmiyte.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lyrogoai.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2aukkfeba.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zwvvmwmg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mjmacbiq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zyqumysg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xovbetit.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tchhqgch.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2odcvkarn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2cnykkcet.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ctzdcjal.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bdlnrptg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2uiurckau.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dkegwdwk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lkuzzrvk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2piziueih.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yvqsffdk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wwzvgxfi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ddpzuyzc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ubsxcojj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fpkolqhv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2pwthbpfy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qgksmbrz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tgdhyqno.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zqyaejrd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2mwrjalgd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2anzrhatd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2oesbwklg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mdwaifzg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ptlvfqwy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gponeyqf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2cakhhlto.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wtnbkykb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vgfomagj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vnlwasmp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fiwunstw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2whrazpak.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2czebhpls.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ygdxabau.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnazlfeb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2brrmxfvj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vbobttre.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rxhgmgda.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lasgfogb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jgygvflx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wrxshflt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pngvtbbf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hiptdzcb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2frvwhpvh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bqxefkto.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jbdtniyz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zibhbwcs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hjhyhumg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2sinskmcv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dcadnejm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gjxhzrty.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rfcqviaq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ymsoyroi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2yepomelt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zpyochlg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jawvyasr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ntkqozkj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nipbtwbe.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2oytlotfr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zrwznulf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gztccwtl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2yaypgvkw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2smpokdgo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gaqulziq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rqhehaij.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2trbyujcq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ctfrtfti.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vvgkswuv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xdkftutk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rusforvg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2djsppyjh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qassomvb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gqkypusz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2uskwmpfy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qdbuckfd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2awtocuge.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yxnlaowd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qdxwtqjs.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wpvjtoww.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mceahflq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2guamqlsw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qpbddhbs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2buesnack.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2hqclbdsr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ejfnjysz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2adpkimzx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xidoegsx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2fnftkoes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uadtqacs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vrethbvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awanklvh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wemtoxal.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2pprejfqn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sevuorlu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2snpjshus.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vkkirgxg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tpsztmxi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nzekuzks.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2oalinlxw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vixvrqce.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pslhcdyk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nprdvexa.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qcegubrc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vwndbwer.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nmgvkgmv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2skvdrnzl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lskirtqn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pkzmuedf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ffpimqjv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yefvvbih.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2zbhrbwce.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2aztwxing.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrhfpwsh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ixnsrnak.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qdbjdnio.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fxjylbrl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kiuusuzc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wdgpxioa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ukrewvpz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nrwamavm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2enbmbmds.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zormqqpt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gveskoio.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2twbmfblp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2stmfgmxk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ntlzrkae.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ocevdshm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2namorhhk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cemxkyqo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxqqasr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2afnkheak.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cpnqwzti.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tknrbpze.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bzpjtsny.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ohnepilb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pwkemoje.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jixgeatq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rixhwaua.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rdgsomzy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qacdchgd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2opxjvbwd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ghnxqhrl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fguvbjcn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2elflvxpy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2llvcutfv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lyltssah.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qnmxadae.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yagspwgu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pbjwwagn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mwpmohfp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ztijuhhb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2svjyokvy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dwxecikl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ejzvtdmq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ibnqcwhp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2jxzqssmc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wcarlbox.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2mygakszo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2apiurqyd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2chyjvsyi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gggnrpfd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tijyucid.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2axtwsgmy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2urxnuqsb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjogjjxl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gbobgbrh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qqjormur.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2itoqatfz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sdslfrmg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lnnlzmip.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2enyfiyxq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zsfbvrsf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2blviohgb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ggdmykbt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ycyarfod.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pbevksih.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ecyyaxlh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zvwuugbl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ywxpnnct.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2annjlpfr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wluaktnp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2pstmcgsk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zqtjwwfa.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2spjazfzs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjwnyhre.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xxfyhvdg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2idfwndbe.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hgaiafqb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdvkrzfl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2epdbiivk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2eohggtzh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2usshmkmf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2pghytfnx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nntaoqfo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqzzehpe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ktpunxdo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2juyuivpz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lolkvdfo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2sjgimbpl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nrgfaeku.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2okxrtzay.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2lobsisdc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oqjoxrwq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2wygosavm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tnjltcsg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yjavevcz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2thjucurk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2svdmmufu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uzavngxq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qmyyvesr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2pqyiiyea.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bywdacvv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ckgtdwch.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nalaumbq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2lkkrbgnr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pisexmzk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fjzjazff.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ytgykrsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqmtfyoy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2iffhkzmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tndscfpz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2agxkohxk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ihdyayad.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rkxneywa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hbzvwpeg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tgxbizib.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jyxmqshz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2uhtexzrc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mknjgyfk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2agmgdvsq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fvrhjenl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zneoxohh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cbwccjod.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jrxqjalv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gjvogqcw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vopmhtfb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dcsxfqhs.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2woooqvmu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2yrciuzar.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vmofqozv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ostgxqkt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gfchmsqw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2pjbkfcun.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pophqxkm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oecaiobq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2eckfcjci.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wutydnge.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2odpdkkhl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sedcltjw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yfbbzsfv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2udgqqtug.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vpvatxza.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2reogzlrz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uvhlsmmz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rfeshdof.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jjrjpqkx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2anetxmcf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2poxggbld.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2brmeqtac.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pxxnadev.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bwbtbgve.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ycshzylq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rjvvrncv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vsfsqopr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xfarvrnc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvlddefp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lzhyvwzu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ijaynyij.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2msxpessu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2bkjumeho.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bajnbaaf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ovqyrbdq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hwjjqazb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gxgyqfjp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2slvkvqgg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fqhdofxs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pcjgntqa.html


<!-- 参考信息 -->