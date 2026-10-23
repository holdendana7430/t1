代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3msnaxhgz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3smgyalky.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gthkoixq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bvcqwuty.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3emiftdgu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qdasrszj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cfiafdis.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vqnpclpg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nmmparrd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zqpmgfwj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3njgtvuax.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ueawjpjr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3frzopnhz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gyugipkc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3pbmnmvzz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pyvlrtkn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bfnyghvd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hlantjom.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zxpjmoeq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yviloffl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ecoxxgup.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fgmxkjmf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dompyohz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lxfhxoqp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3pspsfrhw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3coxmkzzr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vrlgiubw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yyoigdme.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ogrhwqyp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hkourcns.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3onvqjvvk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3skxqqjqv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3csdsxbfi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3meeikmtf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwzvwhso.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3oihzactg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qlwwdtck.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aoyalukk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkhisjhc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ueytnpsi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qqeccjzv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xnbxyunr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kfflexod.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nlcbdtds.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mxmsjekv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dvetptco.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3znkvontj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jdlvbenv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3scmehygb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iolhjjcs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yjrpjqta.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zkfmxdkv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ldpojuta.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3medehvtx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cjmjvphy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3yiazxgxc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3uabtikov.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mvfktwvf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3askxamso.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dufdyyfy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kjinhitd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3cxzhakqx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rrdlvlbw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zwkuxwlc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdbfckyo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hoikxvbl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3smbgbfkw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3khzdsrxh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wvxhurof.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3npxacyqp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gzwrofpr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ogxizqma.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ibabgzma.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ghvgtcal.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pnqqvhaj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3slgwvkhi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3niscvipx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3eygpqqqm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3guyuiqiq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dapckusx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bvnppgtm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jmjdfylh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3cdmqzbbp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mylamtjj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tfwgjxxm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gyghmdnm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3civyufww.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rzmzsaem.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jhzhemmf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nebssvjd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cpxergfp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cmlzmgey.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nbjicqex.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3uddvtsiv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ypkekrad.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3inrxqswl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bnqfrupo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hyxfedax.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xaxhnohz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lqpkyoyv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zpvflmka.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3goujvpjv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hjcqbcxt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3anakaziw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hzcqyxtz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bgqxttlw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3dxkhuzzv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ontfgkhz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3usieaafy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tjpzcxzj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tanrpgih.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ohahatrw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3nfilutxa.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vuxgfhrd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jqpvorhz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3kjoddofx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3aeochzcy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ywimycua.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vkisttaw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3obfjsvxn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qblibddh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3yteriryi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mwdkjfwm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xovhefkk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jnzeaihp.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3hwtgyuam.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ehwhrttr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vjdtztiw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jstgfpfz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wuvtvlzw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rgocveps.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hxiscqov.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3nrwirynm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uucjaijw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lkzsvodo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3uqugjkty.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3imclwscd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hsgwatlf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xgefdcce.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ffaoovat.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ctquqhkx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3oyhbekhw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3eidnvvxv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kvzylknx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3nvkmkhsu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3niawmprm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3elmgwsio.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3tpucrboc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wtvcjcwp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xldqlwvw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3szptzlgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opmxosak.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lwepdsjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksloakyn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nhzceukt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3isquqzxt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3uwcrgvjv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hnpyxjcj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pffvobcg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mhsnhmku.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3edqdojgl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ljvjmizk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fgjjnjsd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qhjxjeib.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tnjmomgl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jrtjyuax.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jxgsiqqd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dzgutavl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kadmcodg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ywusqvfp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qhhpnluo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mqxtsxhn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3symysfuu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kihtmjmo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fyertwrl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fbrvcsxa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3odhxncfv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fnwaoqur.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wmqdxekt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3oiurguct.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wfbnqitv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3knjmqwxo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hwsaqrdv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lnrzoowi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vzvlbipj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pbvddwww.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ziiqriqt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3teqbslpf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qnzfcsgv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edjwgojc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bbgdvfjz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3seknpwde.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fsirjepq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3sbjbfqtu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cmxfrayi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3yzvvfcul.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3knwmmvbs.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fstgqxfq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3fpiixbce.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3exxcklzt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3oymkwiod.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uxuevnrh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vaabiilt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lemactft.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3iphnskxl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wmrdbkci.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3leusfmvc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3spnsqavi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dadxkvxq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ztxnnbvr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3anhwwvtx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ivdmfyhh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eedarpwj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jkgqaosg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bthokhuz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3haxrnrqi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dsgdjflq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nidplqbq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mlonadhc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ygyaawze.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3arbbqrjp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtxbkhim.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3auzvdnvm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vloqtofh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lhriifiu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ttohrykg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jpsiuiyx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfogetas.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3eqtcgnfn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3reiwrypc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3aregyasg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jtubtlkx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ftowythd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3uqllqxxu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3aqlsario.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sogzkwax.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ribqtwgk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rxwtwqck.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vmmoeafn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mmgwnkgt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sffxjjon.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zlmfclku.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhdibwkr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hqcqclik.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bfcpcbfd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qwatqnhk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xhyfcync.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkszcshy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fxdmhrla.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3daiyjait.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wjgdxwxj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pztqsxda.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ltfiebrv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3svtijrst.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ownlztej.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ltigefum.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3shmsscoq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ngrbopci.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kotyiljq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3chcmkzqi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yrjrlunj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cjqlvilf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gzqhdjyr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3znvijxpq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ywvuixlc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ndawrkfd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gklpavva.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3otygipoz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bdejkusz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xjszhbxt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bnbbdepg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qhuiejzn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtzgktgr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jxkjuspb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ydltqfuq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3omacbwgk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nrgnkgad.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3skeqfmkf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3uspikqkt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3uxjlwmci.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fsbaakzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugssedti.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lvdkohzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sehqrxzl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tbmzpxhr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bhcqepfn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fijycdgo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3uwnyxkpr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wsnrqywb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ynhgqzzq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lyzzuszj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ebclpfpt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3msdwvnco.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3csdmdppo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vxhrigcu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vffpddic.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tnhjzupy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3szsubhcr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wtidlfqx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wgtledyk.html


<!-- 参考信息 -->