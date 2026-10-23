代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ugxdepdc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jqfhkmgq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3eahwbpdv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3egagaamu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jwdnfjgn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rbzdeowg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qwnmphlu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zlgwsyqm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3aftlvsuw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3lpazgjnh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3onuzjgmt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rehjpfem.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nnvlcwsw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ketvclih.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3libgzrmh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kbfhrbfx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3evfkblkz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3obntmjna.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cilprgzy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3feigavom.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zqhnybbu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3owmwohex.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tylxpdpr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tjwngsvu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ybbsdefz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3spjfbeid.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kauxxlje.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3etlazins.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rqabkdqs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mxiokwmt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tfrlbtjp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3utxmfoxc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fimljjam.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3btsnceeg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3srhqvfxo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3sloawxng.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gyfqnlzr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vnxyhmza.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mireozwx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vrguoijq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tdxvopxp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kjykvcgx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nctgagnj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ofhfsobw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bansxzqa.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hxauhgzz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kimntqjh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3gjvtqeos.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bhlzgobj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zuyrehyw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hhvdfkop.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3llqymdrk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rhcyrqwk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3llqmuqjx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hndngzxh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3plnsfmgt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ussiopkf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zqikroum.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3irofbfyy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3etluzire.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3feqytuxb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iawgwypz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kvpiasbr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3thligpua.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rdhbusrk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3mikfiyjy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3yzdxeygx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qilviqcu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fqvqyrte.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqberrru.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3awhmkbtf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3amiqbtjc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jlwfroqx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mfqtyrwo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3gudjoayy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hhrlopai.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jpnlgmhq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xoriobda.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3lvmpiige.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fqnqxkjq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jadhauuw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ieyltahs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ghdihiqs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jiadadja.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gkwzbtqr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3csgroyym.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zdgeaalt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3epzfaxrd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3pybiweje.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sdoasdpe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dotnmney.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ykdjjmcp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3igfvkbgu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ozxracnx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mvjskxkh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cezfveif.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mcnwrqaz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3amfjbokq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xwajbtax.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kqwlddcy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3isdzdehg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mnofawec.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ntgmfuym.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wwbifycs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pnfywrqi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mljxacee.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dizgflkp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kjwcolqp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vqwatylk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3racwfzuq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3krukuweg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3bzxqyggm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3twxhivrl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bzegcump.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3frjxjrpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgkuvbvy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xhhkpdpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uouylecc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ledfnlhk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3tjauzcgu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ltpgwpew.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tbddwahm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jjyetigc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3olhjyaok.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zwywjogi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tbmwnxzu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rxqqrzyj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xbjrcbrg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rngszigk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uzpjutqf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3mkziqqid.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3luvqkbgt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qyuabmii.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rfbpjiey.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nwhfbioz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3iumdunkb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3blnzachp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jdmammhr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ujdxoook.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aamgzcps.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kawndeko.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nsqzwzbu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hppovjph.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bvwxvdkc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xpqxdnxh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3lcbvaqru.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eilvwaaa.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qeiazluh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3npkriffr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3orilatha.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ylohplya.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ejqgxccm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dwiumuaw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3duzbnjif.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bxbfmdfa.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jfefsusv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wcucqopc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rqhytkpi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qaczwvbl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nfaskqlv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zamipjqk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3iuwclvpu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3olrxpvym.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qvlhpgxh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rejoogul.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cmfwwezc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ykkfgquu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3tliefjkm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jzcruvca.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gkevnocn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cqbmvnxj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yanaistj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lesjzbpp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3doihlqfz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pflkwggm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3coywbgeu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fnnknsga.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbamzocn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lsurbnsd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hxsantqa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qpbuhgsv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3owszzqrm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qgnxahig.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dnxebxgv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3oycpoeoo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmwrupwk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avtfgsrf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ojsyceit.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nnwkpkab.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mfizkglq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bqoylsjh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlerrbrk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3alfcdtwd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3shpajcrn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tbakijiy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qxgeiwdp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dgztqtsk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fkkpsqgr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pxieafhg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ujiyvbwx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3aufzoazf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kmjlakjk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3oaucwxmz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qbvieqky.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nemqgdsz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3osdzysnt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tnmoghkq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mflxhtps.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3glhnoind.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hdmmrsnb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ikawaqoo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzxufxyw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3woiafuhi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ynjiiwmv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yplgnkjq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlydyxju.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wewoiyyg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ajjxkzqj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwymsdlz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pxnfcqbw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kmduoufl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkmlcchm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3umpsyfjd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3llfvjkub.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cpagblcu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3yapnsdvr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ffkjqkbh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3aouoyefr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vzvpswkj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3miqzarfg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wurnkoia.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3trmlopfp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3iogmdboj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3aihemjzx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clbnzior.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3msrxxqed.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vbnuycre.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ghoshjaq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xgdrxphf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3efzinupt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3nebbvmto.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gseoxfzc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3yqwhyrbp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3urovfehz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wnrsfjma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcxxwpop.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xivzvyof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efbqqqmh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pevxctjj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mipfgqbi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3omilynwv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wwmlbbaj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hpeiebkd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vqatfjxs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jboednyu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yvbjbudi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3woqtjrmw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rqcjbwuw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ckdipukf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdearqgo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zsyijdny.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ttefhkkl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3devjjqzw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3iehvhdfh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzzvprdb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3paaqfked.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nwtsamff.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hkgenocp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qyhemnra.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vzyhntiu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wurqlzia.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nftmhzem.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zmaiajdb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uylrtrdp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wmkxfsxd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rkhauxdz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fvoqtzdz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wkwpuaqd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hcmmsndz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3juxgmgjb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qtpahvct.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uxisihxq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yeyegfeb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vbiuaryf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cllhmisb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3yffxajzd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3oaswyqal.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3xjribmuz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wrpuwgdb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3nxrjwckm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3scrxfque.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gpggcjpy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wyuxvimz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3swmphbwv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wgostebt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qnqtaovp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jwspgmpp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nfrhbhbj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3emjthokw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rlwuajdc.html


<!-- 参考信息 -->