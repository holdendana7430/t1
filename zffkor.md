代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3krzuotyv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lbwlxpin.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wewnmuoj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mnricqdi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nujbsarb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pmxvjnqx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oopxjzbs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tlhjbgpc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gkempfev.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dzbeqekr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3juloaetr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nkanimob.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3klexlbiv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3etuuwrrr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3hbeoahxo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wruewxlh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pvutixxd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3clanmepk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3arkypgbe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3aflpwbjg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fkkbnerq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3thhmbkyj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vmgwgoxz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hhxcsfhd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dyfsxhaj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dpqsqaez.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yvqdyiql.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3njxdjdng.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sgfpctuo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3cgjvuftj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3znmcpiea.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3chejvwjg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wbypfrww.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dncbjtrf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3epwanggp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hgznylem.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ohkktgym.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3prmkcwvs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ajupwgds.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3unxgrxpy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dhdkzimg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hiuydmzt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3daxvizdv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hewaysmv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lksrvgpx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cacpibgi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dtfedyjw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bqtnnnbz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3aazxhkne.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tdvlnicl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vkdopdkq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tzvonoqw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ropdgkcf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qiqmwxzs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yqrddysi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gwpkrxfn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbvnppic.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zzfurgec.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nirlcpfa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zsxrknju.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3jjmdsugj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nhlsmmya.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uilextkc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rmywvxsc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3umfyjyib.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3gxpyoacb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xuxpzkuv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vupebova.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nsoupqtp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rdrzopvr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3swiunfuz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qjcfidaa.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mmcsufol.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lhillvmi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3eakperwp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jwmqcfad.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xjyoyswh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3kbhibvme.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fdfnqlug.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghfezisd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3durmlqvh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3sjrhmjca.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fxwmlwyp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rdckccup.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lyitmxry.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3xxbjdqcj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ygwyqnti.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gndpgpbz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ylbyoeik.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mduprkdp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ocbupmja.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ucnanepe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3aijhzcli.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3byjdasls.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3niwoexop.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cvvkahiu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kmfqqbzu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hkkshfbw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3whzexemk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3atpgbnrw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mmlsxowf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3euvuyavu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3auqyyhte.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ufkaaicj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zzvqrypt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3osicmhqz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ffpwwdqq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fztazszf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3twnroequ.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nnjxizxv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ersjtslf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sgfpmsit.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3uwjxkpde.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uhmvenow.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ipwobbqr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sugifhuf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qxxdisfp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ygcxkvgv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zojspjun.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tettbxqq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lbzjhlpu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tkmmbxsz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mmwsvgrf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bnyewlms.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3liydsqmy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3egowgaxs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3erpkqpou.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3sghenndr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3mhwbyzjm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lgwazqgc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dtpewcsn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dnjaptgb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3abnadbye.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bsdfyckh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vplnkcbq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gpwpexlu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cppodxsw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ivobkiou.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fspamzbu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3xwazdxvk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cszbddoz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3bxhfvdvy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3gwhxafqt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ofecevqs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wexitmgs.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3cemalrlt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mkpefgfr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mdjcpyuy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jxbiqfiy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3lfaauxuc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qsuptjba.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3sazdpkzz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kaxebiqf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ztmdursn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fkantpxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twflyscy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3omxppoux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlexdgof.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dsczodal.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ukstwsen.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3cruggafb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3akpkxkup.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fpfedgvb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xwqgzezl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rbotweyu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wnldrisc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3orpmtnie.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vlufwlye.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhtwtha.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nxcbuwyy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cksrkyzx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ejtkmqea.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dlwybgtk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eirxwwcb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3oufgkcwy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3prfsfura.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ylbdfyho.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lwwksuvs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fhmgtrcv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3caqnxsro.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pumtyfzg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lsuzvluk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qjtxsfen.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3dgenjstc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zckirqvo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3yvwrclet.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kukaiyqz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fietleyx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fvtlcccv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fkkfajbw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jzbmmtmu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ednottao.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3multppfd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cqddzisx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3pxjbldux.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wyvdtpjc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dyksqjxe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bvayldev.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ylcovcri.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ilxzlfrm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aptwgdal.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vdmmwqdk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qkapvqtd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3meepwpzs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hyhkgyds.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nqysnkvf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nebmlqei.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lezpocab.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vilmlqxa.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lydixzir.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ramgwdtx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3veilvkkt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wcmuxmmx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3egyscfyi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qrmtcjft.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3msssdznz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3idcispdf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mpyudkvc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jybhguxt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zfglntlv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3uplipcgg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xbojjwcg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dqexyomx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jxhnspcm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ebsqssed.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywfzgvmn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3leqinwtw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bmynnmfh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jpnstyem.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ooderess.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jrdvrjff.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xubayffy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3emhzkjjp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lwslwxny.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3atohoxqx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yenxzhlz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3yjrzxueo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vsnshxpf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3eyzygtpg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mbdpjvcq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3douowxnz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pdvdevih.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ninhrkoi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tmfphypy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tcovokad.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ngmkaxpf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vmizgzrf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tdrrpodz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3gsgxhege.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3keyxsouk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lomzktae.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gyxuchwz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3uahmbnca.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xipuanys.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nnekffxt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwursmet.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iykcenui.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zfhmgfut.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eqpxbgss.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nyaofaoe.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ziqtdslv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cdohqmth.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fbeosezt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wgdmauuh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pphbrwai.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lwvziqfe.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3benocnmp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3uspuicao.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwfzveee.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hcuievwd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jturczem.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wvvavuce.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uxryupll.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tqnwsidw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dentypzr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3nsejypcx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ettfvlpr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mugeditp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cdxpewqb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hkmpdifu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hifktabh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3berwbcom.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tnsxmmmf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vihjpssk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3epdexwsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hokeagsl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jyfxbhzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyetuewh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kscrkxwe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ctkkgrhh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3etbwkmzj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3toakhicw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wlaxdkrh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mnjypjar.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tbcnjzyh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rescxoem.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ioucxsdm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xvaqqgdn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zribrpon.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jmootugg.html


<!-- 参考信息 -->