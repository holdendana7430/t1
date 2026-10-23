代发 wailian999

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3evmuofve.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ipgsylni.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zeqyajxp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3jixudsek.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ikmvmwin.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bxfjoajk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3pgrpetxu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kvzvcyjl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vxyksywd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tsxxcedw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gmkzsrjh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ykbwthzk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3sqvhmcgp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dbioznht.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gfaqzslh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cohdlwag.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bcaxlzqm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cmzqgmuk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vwymmkhe.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xpebjiml.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3mhgrnhfy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wwltivum.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jfwowfrs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sgcmrvnc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pizluzuv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3panbqifq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gvnowvtp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tdmhlfvr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rqknxxny.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3sgvdffev.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wirnsskh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uqvinmhg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bxusufbn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vxvaypfa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3shgqzslj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kydspbwu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cygsptmw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3apwfrtbm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3xawdwbeu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sjsurauc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3driujbcj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vbdubtbb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gexmagjs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bkojurvn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lvishnil.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cmpcntoq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3txxeobcx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3teaggsix.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3phcgusov.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aemlvffh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gtpkgnge.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tunbvhqn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wzqznaer.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yotkninh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qcexnthb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zryaosae.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qprllfqz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gvxwivaw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wapomnxh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3purlumoe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kwvwruhb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dlpgavdx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ywlpblve.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3opskixci.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxkswvqj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3dnheexfl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnzifinf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fffpdlyd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jjjkcsxn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3sspqdxfw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cqyeozdi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3szjakjsa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3snqleirb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hejqllmw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3vxhswgeg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vbucvppd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jbzqkgwr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qooibyye.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wnbqbflf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3chuyanhk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kzxcrfhb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ijcgeewf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xkknuqnj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nfbdbsmg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qpyfwrzs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3aryjawkw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bsqeucmm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3snbfyekm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ypcogvlw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gflrfjxf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jodwdsqx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fekknhrd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bkbhnrvl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fgaeqhum.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3belnfvpi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3iikaqirn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3csmqfcog.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gbczwsqn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3elcqdbvg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3frxvgaga.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bnsspslc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wuystdgo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zpximvqc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xqvolazw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3rscqefri.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pwnewqvg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fvjcdgdt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jfrhetsh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ipusuykz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3nfdrlefd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3djktfbcy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3klcbjwrm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lnowsgcv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3oeagfqkj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3diolhtlp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mvbtmeyd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rihkjjrk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hiausccx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mfiwvmeh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vcdaduec.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qjeevzpp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bvofcfqx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3klkpvukg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rxlvljzg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wfbtmotj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3laetmyyx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fudcwonh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fggrllfq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ialqckgm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ehubmqbf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ztxfdtgw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tpessukd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zzdzmmfr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iodrafqp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rnxnhjbz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3aeezkite.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rxfdbrqt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ezdjdfdz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ankiuffq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3mbgbfaok.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gfynodxy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yfldhhue.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ixgizdrb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ypunooou.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3iklcnfzo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vomwoozu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uvdctorl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3iaitmbfw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qxwzpmbq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zwbpnosu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3kfuofsfc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3aciixatj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mazizing.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3sswmwzgx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yzcjjatq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3uoabrgmy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gyuzphmm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3elhsedin.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3inabmlwm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lktwewbi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3gtjajdkf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3uizbabkt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lyphlaia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etucayqv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dzlknjwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrvohvjv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qbggcmqr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3tirdxawi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hvvqxdyz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ngoupnwg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wxjomkhz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gqhejzky.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qgljnicf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ximxjzkc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3epdnbqud.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lsqgzwxd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3unmatuda.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ojyampjt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3edbrqjdd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cebbiyzx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fxedafvl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tnjxyddw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cjhlipnj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yrumedvh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rcrfnbjg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kztnjyck.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ljufoilv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3desvlpaq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vnleqlfo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xgpvuuzn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ofkjftlk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mkghhdjq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3enneqjze.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mguvqyef.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3llhpntfc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uxweurcb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vfxpzepj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vtpmigzy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vbpebhaa.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ecidzvzp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fzymzaej.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pwygrmgc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3isuhcnoq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rjxhhgbn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ajejfxki.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wtcswfuk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3obwrleqs.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bzkotzlr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hwmjtnfb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vymckond.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ebmilybu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gpuhgyrz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gwquwesc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3addeqtsw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zyqedone.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3najvcyjc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dcbetiyc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yzmagyah.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ujxthcvd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kelhubvg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zmxqubjv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dqucisqh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rlkzkzbk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vtqucnem.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pzucoite.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhwvszdw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qaskjciv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vbeazlzo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3esdepzem.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3blrsdeoy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rkrqgwtl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aqwuzgtr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3okwyteoc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvezluku.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rzjaujrl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3uoxjczzo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bstppykc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nujtmrhr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mdgqpnnb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3epscikfb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ijqibdje.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jmrsqjqh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3dhxqqkar.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mxskwxbg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sjshtdmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rpubcqer.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zqpejlxx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tmfkacjy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3quygqrxt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3yftdwawh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mahdliik.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qhhtmpaf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gfkdbedr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ljtusfrw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ljpyeeru.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ywzzxovi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3exqxfxqf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3moemcoky.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ellqvpxn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xsyjndsn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wpftuyia.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3jwwfdrgi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qhbthdfs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3okhlqgld.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3likmwxwi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xmwudodd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jtjhkfqh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bsrxcxhl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ncbqyurw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xckuntzv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kifghdwb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jfbbpfzj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nmqtiavu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xhoysyoo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qdaiknry.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xiuspnde.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vflqggqa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3bnnzhdms.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dkdugmnl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pviwmvfe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yxacsdzw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3klaesesy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gmqzqjjs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3plxwheci.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gfudwwex.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3yaxoaqgz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ofwxqucr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3btndrdgk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3dyqgcxvr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3uggfhmqm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jjgwpjwy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3akihuqms.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bbcqbcet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doboyvbn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3eyeybryv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plunkmxu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tbkqqnru.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3itkxuggk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mraprupr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3efcaesaj.html


<!-- 参考信息 -->