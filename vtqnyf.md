代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3huihoezf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3okdaewan.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3atdzqrlo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3rycklqcb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ikdoaqwb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3obzmlekk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nemxrfbg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwpvakmk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3egesvybu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3beyndqjf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nhswxeie.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3neyrzfzx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ilyjktlr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zmmlqgvx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vthpiowc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ampwejtp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3etguobnu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3chwvfund.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wukjmtya.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3akefzldo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xzqcwbgy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mrkrsnvv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3atgzmfgq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qpxlsmfy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ykhnuxln.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hmevecif.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cqrnpods.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ktkwmknr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wmuiissq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3byopxsqi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vbcudvuk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3uesdvspp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3cdsrcdna.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qguxmtex.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zmjzjbno.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oslnmnli.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3opykilaj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gpvqfmpt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aggwnpme.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gbnooavu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lvvetcxh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3smtaxteu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nglvrrmr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gmcfypap.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fiplbgxl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3adjgoprk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3shfqsdmi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tpnyeivi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubxexzrl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3izptbdwx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3crbqksqj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3voetctnq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3uiiylfkn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ipuodlbx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3prfzjolk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ieqdsyym.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nwneuory.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3esznukqz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cxbihyor.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3cgfdkpuw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3wasaowxz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gzgpvvne.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwwybjva.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gocgmwkd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gmikbnls.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gyxdqlay.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rbznmave.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wbjhohpq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3diioqakt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lgxkoiet.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cxjskbgc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zulspsza.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lhljtefp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3alwdttba.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ubsehsgh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3zvocesza.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zxnrjmrn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3madnupqo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gsfekome.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3orslovqi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gbmxbcpt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3cexqskhn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bkgmamec.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fyaijzvt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ahqjoovq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vvgxfimj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ttqhjwee.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3leokppbk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sswznmhv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wfhfjktv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ibkcfbpv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3moyulbdz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3icsdrvhm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rkirmuxv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hkbkshvf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dojgjyqu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3abxvgwih.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ilsofkrj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mxverqll.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3erxbjcjn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lemtlgve.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nlsccfmw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dttvkbgy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3anmvvhgc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qsbdmebh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3aomjtecz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vjhjonnm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qqoguoid.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mjkorhjo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mgbssqgr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3vpcwttsn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pktfumlo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3otnksiak.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xyutwnsp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mwgfgowg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mkolabeg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yvcfqdhy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vvoancbf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rbtydubp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yzdnlbct.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fblktdtn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vuvbdijm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3lagtuqiy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3pdbvvvva.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pimxefkx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wfzxdjcu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xvbblhaf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3avoyhyhj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kirwbidp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3iipuwgjo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dhkyctoh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3eiwhjyvh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dlxqkrko.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3iaukbaed.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fggxbbif.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wzkuslhz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kvuakwnf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kjfytfia.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hftdbsqy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qmrozyjp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3frirgunx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hpavjpds.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vzzggyvx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gryyocwj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ktirpcis.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3oefplxzz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lqraxwkg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tvgekmqu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vytgfgwz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3pxlevdqd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yleaflql.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gexsisak.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dibfhwxl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rhdnparc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vwtlfydk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3yyxpemxg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xqjygrng.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gpwwamhr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3khwtbjgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewuzpicc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ilmrbknn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chsniyjh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fjkarfqf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3oyiwgrom.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qedsgvqc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dmigucua.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ncowknrk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3owawsmeh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vkubiamv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ersnuyur.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ugdorros.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wokquqxn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgoziptm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lxeoiyxd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3liukakrh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3msaadmtd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zqrpujhn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hjivrfef.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ydrlgpmv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gfmsxitk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xgukzfge.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jbrsesvj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3heqehsen.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjbwspvr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3keaakgjj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3gquharwp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tfwrxhwg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hbtqfqvw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bfjcghzc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bnmqaaaf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qollcehz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3msfegtas.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kgatniaf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zjcnufug.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ecraxyjv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mztniwfj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3eqzmpvgs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lciuzhfi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3yxcpbtnz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3naqsvvyw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fnsiasdl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xxilcqtv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3khpfgjfe.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3panviqmx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rjnmwals.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rulmplys.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3becbnsms.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rreocfxz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ozqjctlm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qfapwvja.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vyioceyx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pcabdccb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vgtkufyo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mkquwkoo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3slypmnna.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lvbdgiya.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mlmqoggu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ehzhxtea.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lapwaviu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jtiotvtj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qavpmisu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tdvdlbdr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zlezjsni.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jnwerzow.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xdygqpgq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qlrsvmsf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wisdacro.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3conwkedm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wvlejdxj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiphhutx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3bwiuwzke.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3cfafrjjm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ivjckiyr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wvpqwhkj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3rwdxgdao.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooatevxi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3eocskpxf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hqoiuilo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jknetlly.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qvkqshnm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jfmqvikh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3benqffdi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jxbmskyo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jkqvutwu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bnoyxdiw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yrcqpaxv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ljbuacyw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zhwkhnfz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kcgveqip.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3iybcyimd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ugbterpj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lfdftdbd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hfaqkmfy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3btclzklt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3aralvooi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhpqlobc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3cxgyitfg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3exjpmbqx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3pfkvpsmf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kfpxnpoa.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nycpxieh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxnyrdyd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxezswbf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ydvvxspf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hegymdke.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxenwebc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cojtlpev.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pqwktxvm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lxfpxaol.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gyyxarfq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rtnpzmaf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wzquwkau.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dkwelwep.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fxenywih.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mjsscblp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3aidhlsue.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mrzwuxed.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hliizcam.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kpmpvcwm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kpngzwhi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3iqvudwkj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wwphsswu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ponrdjdi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ladowqmk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3euxrrmoa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lkqcutcu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jmuysozu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3avaidocb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tqcszjgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhwebhtb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vjiuqgjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gabaufdu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pdgojcaf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3shgkenkp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fdzzmlad.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gvcdagee.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3inbxkteq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bybbihnb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3izrzfqlx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rkughtoj.html


<!-- 参考信息 -->