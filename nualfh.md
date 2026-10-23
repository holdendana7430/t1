代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nrqyouoj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3btwpwxdt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dvvnvenh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ckilewjf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3fxaohqvc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mmwcpckj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dkxjaiql.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jikxbkuj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zlhvqbnz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dnlgpitj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qessgdwq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3okeeafty.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rxdkefbt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rxrnonet.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cnkphntv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ycsxjbro.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyvjokjn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jeczxobc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qkdvrepv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zgkhgutn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3avevutzh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xxszgdmo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gnzofkvz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ztfasakt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gtxrpkzi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3glmucgwi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xplmmwix.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kreceaya.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ynjbeiqi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cjaeiyfm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3viddbrmc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rdgwkjrh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hdixfvse.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bljxvgnw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3urzxnqxg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dpiqrdhb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mhzhmwke.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kayhxazf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3dbeyylgm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkbnknnz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3xuntevvr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vgzevibi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wllidykr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xbmyxnvx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xptxbohm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xovrynpb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3eitsbccv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3milrcdgx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3njzgpdcm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fsfshzau.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xvbhdeoh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3rqjbwdmc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3smgeknoh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hgwvuisz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fpecaumo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ojjbwkxq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3itlhpdvq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3urluzcpa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xxryjznt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3brdxkesj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3utnpncpf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jalufxst.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dtisuayr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wnnrtzpe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3nsqcrjnz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xmeqeogh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3czofufod.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vtuivrnm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3przhmsla.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qjdpolzq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mfksclbi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jifjpgry.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3irhifwyf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jaductgg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3sgpbzloh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wbfnmdjs.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xrbhjauz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ibgekkcv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xlconsaz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3agwlwmqx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zlicmcbl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tsxzryol.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cqahmair.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jofvwydw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3svmycldy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jrxlxjvu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3mezipgdb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3osgmvjwn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jvkqamzl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yddbnfhx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3huyzldow.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3utnnatny.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mwwfljas.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3copiofgl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tvblohhn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3itrgfdii.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yheflkze.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vfvnnvol.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3akhrlehz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3edetungd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bjkbgtee.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hbhcgcoc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qnaivdix.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rvzfseyz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qchidocs.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mkphkxna.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mkwgpbxc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vrswfdwg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vyibkcsv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ymrxotgr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3slghfknn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3oauncmrb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wfvvebwg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xljwnzcs.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xagywpcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdtpuxly.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3plxctope.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aoupkcht.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3irskvrko.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nbojfpfc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wklcvcrb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wqknqvtq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bqsvlhky.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pbwdbzno.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jywgqaum.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xcgyxyyu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jqcltqwz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3klsaksrw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ytsqgjsn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kovmkkjo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lpxfxyqv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3sssdgxrw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3nsfkhreg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3bisuphaf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pborsjpt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kjwwmftt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3bmrjzjwu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xawequsl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3oilswnkg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uyedleay.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hvwyiayp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3obkwkkuh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zviqtppd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3awlvjicj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rycydmef.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3empbtwlb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3caakmvgd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cvhazvyc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qdhkbewo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qdgxvpum.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bbmrajpc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vaweqkul.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wtwmszmx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3grqsarpl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3odswxinu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lxjzvzou.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3iyvqfsgt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3djcrxmog.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qoodqljv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3abmbbrgs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ozsfbcch.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dzafhjob.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wdvbtftj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fwbisllk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vkwqnzcq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qfalobkd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ecicvdny.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ypdthtjq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dxsqdciv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vlghnjnd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3iyubumzi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qrdwbkez.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fjjhuczt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pozyplgi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ezriroxm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wdhgqenn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zljptqbb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wuoysenv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3csiurwvx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3llttrflb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3disiwbep.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3oxhgjyol.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3eywktmyk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3svciumlt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rvuixlft.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3uzfirzin.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dadwraku.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dpqqzqpz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dhcaapos.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3uttjbmpu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zdwfdqiu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqncjbbd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dtirqjgg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bkbgcnfh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uueritpm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fmifasgt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ovqltbhi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oizbrmbv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ocmkcoxn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nnepgvab.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3csemqofq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3awwjkxfh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dgixopsf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jcwmjzps.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihtjkyzw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3bvjimnxe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3whbzeegl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pbqphham.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ckvebeub.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3yzljiiao.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ejqvqdsw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3unuekbac.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3kscbkjil.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ovpsxoes.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cduqetnh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wbegeuzb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wjmjlope.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qguhlxdz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cclxjeje.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3retrwgya.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fpmcfhfm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqcarkba.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sismotkr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fivjicji.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yhhyuofk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xclybnpr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jmmjgpoa.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eszcdgus.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3quuebvhr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3voslvdkj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rihzuhol.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vdssqias.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wzueozpq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sxdenbbd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dyamduwx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jnjbbsvh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3oyknjcvk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qdhzxcal.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zxafubdy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3swwtuqnv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ehasqhda.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nlampgpr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tzgzjqjg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3leffbbuj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3phbjirtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fymopoll.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zvbemwwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgawscor.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ewuxqqdq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3shkudxol.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nrysiuwt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yqeqontm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tigueqda.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jykbxvlu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rabfudso.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3whuidvko.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qyubnyvq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xcdpjoxz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ehiaejdc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nwbmjucj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vlbtaluy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3njupywzf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3buzrgdih.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zbrncpic.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mvivazvk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ahlpbfyx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3uwxobsqa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3djpcrgap.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zouwxbqx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hbnedihh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cttyesom.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rfgbeoti.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3uhbtnyng.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvgrauqc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hsjmxfjl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lfftwzsf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wblmvbia.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nlnsmwtn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qbftivrs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mjbnulnk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3yeqekagd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lcgsnvrb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pqdveele.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hmvqatkc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3olwybnmo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xnpuaple.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zxpfsibs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zrakmakt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3enmfrsrv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3glxaygwj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rsyqngpm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rhfytdac.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3adelsmmt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nmqedecu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ckfswtoq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rzaugoli.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hzinsqxe.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gyrqnkjg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3cgyzyhgs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3caufyjxi.html


<!-- 参考信息 -->