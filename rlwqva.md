代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jtavfwrf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tprywhet.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2bzquzfjt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fygedbej.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kralxhqi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nrlyyuvh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lnounvsy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kstonwew.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wlbipqkj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cjyasyur.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2clwvqiku.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2snnxlxro.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2oakjgcwn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gywjjkgg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ihycguqw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2olssbovv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yuleekfh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hnzasfoy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ileqdspt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kngpbddh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yypbulca.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2gqjeyzbp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rggdwjzw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hbbgwsiq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqcwevwr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vqaaalhy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2brognfgg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hbghqoja.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zdlkbzwz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2osaadobj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mkappwns.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tjoxjohz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nrpxkjgd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vhjxsqsr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xwkaolzm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qhojcwtx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rebtysxk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gpmrzkdr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cgmtvail.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxetjetr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rnpylhyy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2urwcaeqg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wiokzprj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ywskmarr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hlspbaxs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jnldappo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lripkmui.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2lccwruuv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jxyimhii.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vmocnmfb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mnerfaga.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jbkfsvzg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2djfabjmj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ivutstif.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2iynzktpn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rlnertbe.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fppdilhn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ccgxspbb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2aauxvmjd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2kveizapy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fywepagu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2iyteimgl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2kqagsgce.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nauzmmnq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tycvqpab.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wufzxyso.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vvcpqefn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2txjzyjrf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vrgtzjgl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2aashnapg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yxbydres.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2clrcuskt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ygpjzgmw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xrjuhrqp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kupqijah.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qxufuoiu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jerasgfb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ujkeuvpl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aaacslaf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cgoxvtss.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mfsgtwyz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2fqcwxhbv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rmbnarko.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2aogcitap.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wwjhymom.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2djieizlm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wgfxepqe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xcgfxxrp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fmpsnioy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hlwifgnn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2icpvkqjz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wqtptpgv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jopmlski.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iskgmnfk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2sfjlyfgi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lyfgjyhy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wgtbbxuy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mnoowjgd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2glzkfuej.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tcbfvpdl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2eremmpdl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tfikmhwy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2itgbfrdd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pgovjykl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cokpiozv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kxhxauvz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jwecjnfo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2repegups.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nhewsdgw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dxixgetu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2woxzuqky.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lpocedba.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2renizalu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2elctigar.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2sfnkamzi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wgvsosyv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2yidhdbql.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2puvesaez.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ozzmvnci.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tcnqqmin.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nxjrfdsj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2moytrfpj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2evtudwvu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qwkhhwog.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bvzncboh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jcvgxltb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jpuorytr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ihdypnrb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2htgzmibu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lhtpkalm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2irmzfejf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hqrihpzs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2pmfyibuc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2evbttvig.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vvonygvh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2iopeavuj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mlitxanf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kclghsue.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2eyckvivl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hmtnueks.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rmctjvwp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qzbnncea.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2qfattmry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhlcvpds.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rpnhdcoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqwumkvc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2moftcdlg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2npmotvpj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjjqpxpn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2egymgqbd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xenkjvop.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2gelcknbp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mhlyofkb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xklmyvul.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qogwpvkq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2snbkxzdx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eeqfqdjb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2urrglciv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wvfeddhg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tveqqvsz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hpkgurlb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lvedhasz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rpovgyop.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hneqjvnl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2abuoqxin.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qjbwfrxv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2opkajdog.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gppylnqr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pwayfeoj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2jcneqtzi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ksmgslyj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bggfibnn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zzqccaal.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qbqlytlj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2brkqwbpy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jpkhwgmw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nzhuhlgi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jzxmgtvu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2eqkmgkqr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gsffrmbt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kqtnersy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtbfeunp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2iittphvx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bxdiuskz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ybkziciw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2eqrmsoiw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2daigkusa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xawmuyuf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sryubptt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2foiezijg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2otcdugha.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2eaxrisak.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2krhpzvld.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lhetpoig.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fznunuhr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kxwnuasu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fulrrtdh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xewaznms.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zzosykdw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2lafulezz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kacfdhyj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fiurbxvj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2utxitbek.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wfubpzrh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zstrutbi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2fggwnoxp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pzeqnutw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2iohrsgwe.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2adydhafr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qqkgxtmi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qdbbfcpy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rshyzzva.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jidioppb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ysnswhpc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qppmhkiv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uznprrmp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vcwlxiqk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xfxhrthb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vooziycj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kjyfkvte.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2aziendqd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nrwerifn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fdnsyhhr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lptokyvd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hmzdtzjr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rvbcjgwj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cvuqydkq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vknucoah.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bqesdknq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ahyjthwq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wdwfvgkb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yzjrkzsp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kplgjrmk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2manzukkx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ybcesegd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vegankyw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2quopvnxz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gyjqjbkn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2fqmgxnry.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydarumdb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jnhdualk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2eolftnuo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vnoxxqok.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dolblaob.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jcdwgpop.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2uhjapehc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cogbeisq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fzhizire.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pwzfiosk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tohztost.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yealrjtx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tbeyffaz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dicwnqqj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mglophhs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2eisarafw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vaychfao.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cfculsso.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nzjctutk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tjwkksno.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wnltuktx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nddrkhxf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kqicadne.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fxedprkh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mhijldnl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lotfcalo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2erldpdms.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xytdvbkz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2bxtdhyxv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zsfvuiuh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zbfdmuoa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2uxifkuqc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2lgronnli.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vnmpihhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plmhwjps.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tzhudowl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdmwfvfm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rtamyidu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2azegaugb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ieosutcn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2idlbehra.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ikooqzom.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nptwjyzs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2oetsdmdv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2blczkmia.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2labhpugo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wvcmuitz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bjqczcbi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qtnvaaym.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fhigdrkb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qxgxygfa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ljxujpcl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dcicobuv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cvhqdmdq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fraiznbt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2lfamxftw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dxvviybk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2htccnikb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bfbzramn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ytcskrff.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynuunxoo.html


<!-- 参考信息 -->