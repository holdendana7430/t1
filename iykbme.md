代发 wailian999

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vdpabnqm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vphvcrba.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wwyhhzry.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3honxaqgo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cdwylzze.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cercuyqf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pvwchtiq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3exfkklwt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3uyvndktt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ckmypdcq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghaiwwgl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ikyvrvir.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qsmbzmsg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qpehbtxp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wqtfruwn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3roexxtnu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ucirpytw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3azwahlnr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vcdjpawa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mddbiqym.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wmzshceo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uvlldtfy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3aslnwiij.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3sqdbcdsp.html

esac
来源：http://www.52xcode.cn/Article/details/gt3uzshruqg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfeccprx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vhqpdwwm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lflsymyw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ksixqqfo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pmjupbwg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3iiaxskxp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fjoixvnw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3tqewcolp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3frnqqtqu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eetjlozj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qqmisdmq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rdzpxaqx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3gpelyhow.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3acsnxmfo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tyljcbab.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ltsnhwfu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3otovgqlo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ywuwbpjz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3crkcrwmz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3owrlscju.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ruhlviuo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yiqomoga.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ohuminmj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qskmcydu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zmwkuugx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3inuedwhj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rmlxojqe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3eljbvbxo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yeypetku.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cavmbprb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yypsjxox.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3aszudtek.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3afsusaqn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gvsqykdb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lklipdqj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qgumbznx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bmdbcdee.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gzuufnkr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mdscwrkz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oatftytl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ndmoccdr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdyqdsff.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3oqcisslt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mihnldqh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3kohsfdjs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fwnbwzxu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3voegagmy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vsfeqggk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kmwzwlcf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lwskbthf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3btbkqjce.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vldjfbpm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3sgfmoclg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3maeuegdb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lsyfyrvj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uxandyle.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cmqfskmd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dzpgpmza.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jdaupbsu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vuawwrcv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rvfdubra.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gapsubpj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3oriqpdxp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3udkdbkmh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fjdnvpau.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cmlqkniu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vfgytnhg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mrrjgsxq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3orgaqrir.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3brcvxamq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3oabquokx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ifyguuwl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cnvvfvbo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pnmzwwsj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zpaklkop.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3osqilekb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3muuehrfc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vvfrxbdc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tvljjdsw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bhunygzi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qvnytnuu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3utzrumlo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3elxqvgmu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rbkrgnfl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mhcoqpgk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zvpbdhfy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xfpvakiy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3digafjyk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cdyidngy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bnqmuuzl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bjjnhvbr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3loqbweyg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3yhwvgvud.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3potbcatm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ykssfzhg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3swheawbx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3grujvdzm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rysbnhpk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nfwmobhs.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hypduunx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3clszytrg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3lesbyfzi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3uffznczp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3skoxdegh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lrbastto.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3eumlbphe.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vkwkbfqt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vggelfki.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mzjlxueb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3imyecnlh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rjwxfqxa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3geemwbkh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mlgokqrb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3frvryxtu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tuuzinfo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jwloddqr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wawljsez.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wispjexw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xfidswjn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3adfkjktr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kkwculli.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3micssjup.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lkaypgfu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3highfpcg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cbrhdxzg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qydsxpxf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ejczsddo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vjrcdnvu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xybergdg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ttkfnmgq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3yumgirkj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3eptsvcwg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dntpcxbw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zcpsknnf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3badaizbm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3iwtnuktm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wyifihxb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zlgmxyfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfapqltm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3angmwyzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntmyunoj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cutdcwht.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gmlrrgzz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zbmiyvsr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qalprsru.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3yygxlpyo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rqaoyrbk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3epqtwsvj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fhmyhhih.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3eegweeuy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3olvjzmoo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3apjhnsbv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ossjspjr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nrbdofdy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3irjgztxn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vhgwwoji.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kiegkrij.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kxeasmjt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rhoqaakr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3sxfjqpln.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rporxjqh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aprwuhfy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3brwtaygs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dapamazb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ftjydigq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qecvxxzq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwynhddr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bewceovx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tuvfnogg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3shrkuuar.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ymrveegq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3abymifpn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bgiwadct.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3axfujqpz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3whfkmeus.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vdxjvywi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nuidbukq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3sciqlrwo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mnpittvz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zqgzxypn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wbvjmsbj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uxbqquee.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gpljuzcs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yfaqoozs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3psnnwtgx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mfkellyp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3byknskri.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bnpkahbf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3uxiwhgce.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3exghxgoj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3anyfxofi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3unrsrhvm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ijqmhpxh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xmhcpoxe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rcuitksa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3lkmbdngk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3sadloeoj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3stqvzosb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jvvgdqqz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3krrujpaj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3oaarwddq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kbwdckkh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3gamfsokj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3yovatqgs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3klahndxj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3elizskqz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uhlvtquq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ainjtjgz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kpdzzoxx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nmsdhtdn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nfrlztwl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ebphwngf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eqoaejxa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ycrnorch.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yhwcmmve.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wxodhrec.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jdydlznr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dhbovgub.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ixnpxkqe.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hflvmyas.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3elcoitfu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3evbketum.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cbymqzet.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lgijjrfi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jybseshp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xwwhkogx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rutzunpa.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tkfxlnmq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3agimvicz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wuovcvsf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mfplbqab.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jntsyngw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ixqyvptv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3omdttegg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpssbjnp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zmkkoxsd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3osaxqmdr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yazmnbgs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vbrousyo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3uqpxpybm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dstpuxba.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxcneyqk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3auelxwkz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3unhlaedk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qywleamc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tonwglra.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qkckuhdi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wcvogxya.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3blvmvflt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rjzxerpt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jcdgwlbu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3oezpnbey.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3axmbqwnl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gsmvejhj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ucqnloky.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3peklpbmy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uyosgwnz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kpnzlppp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3qjaqdyoi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bleowead.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ddnkwyyb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3eibpprnb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wcunzhsh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ziwxausz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3pemiqsyh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3iympuvex.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ytdbzerd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wmopkjqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjbmxeuc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zfybslnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syvhgijd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sicfopgf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mmhpcvpw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vjbfdozg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3iajuylbd.html


<!-- 参考信息 -->