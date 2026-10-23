代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3okahqavu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3egrqdeza.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3coxdwhci.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3glmodkev.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aptcxfiv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nzjrjgcn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fqmbwkuq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vxvzvwpj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cwtrmpyl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3awduikgk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dcrgwixu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dbgmckzi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ttnmrzab.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tuabyczk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ixaidrre.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jgwcwpsk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3zknkgksn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bcahkzcx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuikijrz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uoajkqcs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3xrqydrzw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gvtaayvp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nilurxps.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xfgbeytf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3geodhvaz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gtzhempp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3lgttmztv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ivymhhbq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3lzcdeljw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zfpmcfwj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3sgaerwfm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnbvhjwr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mekapsec.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3pqpqajdb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bmjtykdo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3aduiizzi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3anctdzpj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ozydgcbp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kirfjumz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zraqfaom.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lykooism.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ojsxycqr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lykzdzwf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3gqzvnwsn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dppjssiw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3exjtjzke.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ewnnjtxp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pjgviuvm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwuhwfk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bihsvmzd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kwalawib.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gkpyuljo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3snxciwlk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rrydjzla.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3cxfdhpta.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3uycsslle.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dcdelmdc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3kajonzmh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ducpbmdi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3maeacxys.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vvulcufi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mbifmgcl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3edfejedj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3txlzbekq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zsbatidp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hkycdcud.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xanesvyh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3luvntnaf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fmhissxj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ektilmtt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jtwmzqfi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hcpgvzhr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3gpbvlwab.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3trkmlods.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kmdntbbq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wcmhvefy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vfaxjzsq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ssfzzkvk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3cujrybgx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3trrtoglh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3aitcpgub.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yokutzvn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ledttwlw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jjxumxyb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3iemxecky.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kocecqot.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ielqrbmp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ocyrwyze.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3niicjisd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppzktots.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hhpacrxz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qzbayypc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kvwvnfht.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fijiwkpt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3tevcqxeh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3gkyidwpq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nietnkub.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zyvidrrq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hlxnjvcd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3szkemetz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ymnlpetp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bxvrnyka.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3crhcufef.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bhydajkp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yaehptej.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bwdfvvzt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xksylvhc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3acobqsgu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kupksjwt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gmzcdims.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fwouuwag.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fnnioiuz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gxdwhxrg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3umnjymux.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ffgyxtep.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrtwwwis.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gsycufrw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3raobnmhs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ndekkuoo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nfobnght.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3srbryggb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3iuxwaxcy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hadnyjbk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hmekmkid.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zmocqerl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3staofbng.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wdnodygz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wzsjjwxo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3etdpcuds.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wynvyulq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nqvjwqrt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lvzpxiif.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3obzwhfmw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wjwwyfrz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mftsicmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxgzwxll.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yeoldsal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekcqcncm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eprxfesy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3grstotdm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vyvexhlt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fliuaetj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rzkyjddl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mlblzrii.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3enfehhnp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3stqlajum.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zymvjjwj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sclemhqg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tmirkzfu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pclhenxl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3yppodhja.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3toqxxupn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rcoclleb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hnxyekwn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vbwwtule.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ybncubqf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gaubojch.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3fmcyzzym.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3iwyffcai.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pmlzqxpv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ywtpayhe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mpxzxpba.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iyuhcfyl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgpsigrg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gklmmzgy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zaafrenr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3uhktkyew.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pgayhrbl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dqaclgxd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ucmsrfms.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3chhojdyt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3blnygxst.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3otyhyiwp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qsyuojai.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3iyyjlynx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qibiuwnk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jzuqinpo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3kxztvmpg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zniufkze.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jvkwryio.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qbpjvhlu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rwgsvgjq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3lxuawcwf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3najmgzao.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3luqszuuw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oemmptsu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3copaghat.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mnuaogdu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zapzvybp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ibmfluzw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kcuoyhft.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sreiehbj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3emoaveum.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jmqxbvyj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jrtlpgei.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3whniufwi.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bvddiled.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lykvxrxd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wbfhsogj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3dalszoyk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3apkssyvh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bdzpgfuz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zdkxdrml.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tiryubpd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cyujrvnm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaywbghd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vnzabtwv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3whushkie.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rqcvvlei.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3anhljbua.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bofzuryp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3loonlbea.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lqfwpelt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cqytxsst.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3oifsssfb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vnnxrxou.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kzggjybj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ymjcjcqo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wqqgdtfr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lkrywqgr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mjlgmhbo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3snghlubp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rknqgqqq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ncwmnnla.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ufgxusaw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pyftbpkn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qsnhahsl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3lxvqvnvk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vdgczpoh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nfrprxrs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tsrbkhxj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dbyzewvh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hlmsutbr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3amykjuvn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3koawyvtn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfvuvduv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wnarpkxz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wyprkvou.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbwaeqdj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3arkvihue.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mhhfivph.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vfiumbim.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3afbhzltm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nxvtrlqs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ogskysva.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xayoyocm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jnthmlpw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jwvyjksw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ytzrkpsn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hiyndfro.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3whbsvdng.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wdlxbjaz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3amvuqrkw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qekbywgv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dwqcgtsj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ihbvvveb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tapzrfsq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ykpsjxqr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3obdozabs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rnrtwjqr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xzhjvgqm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ddnlkrnq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dqbkxhrt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fnvehmmt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fzbnseuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anzhtvma.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3retlfiig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtrmrnay.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bvkwjcxj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oldetftl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wlvudazo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3blqdwqmr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lramcdjm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xhlkwjni.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3uoabskvc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zvbgberr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wwpzbfei.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ztyeniyh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xvzcyitx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3brawlcum.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fnvcytoq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nhbgckre.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3byzvwvat.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ruwxqqyt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cqcsycfv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xkjxhiyk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlzznkot.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vntnlvbw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dwhrodph.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3oughdgvb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jgdnwwod.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3isngqauh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3imgrcagw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fonreiwd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3enfyevgi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vkmhojng.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qosqttda.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3icjamgit.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3plljrmdw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wauuwaib.html


<!-- 参考信息 -->