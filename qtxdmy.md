代发 wailian999

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hpzfepoo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2azwntdjq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2pustwkvr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dtcvpayl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tgpiamdr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2yqjgpwrr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bmqtyyus.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ukpkhhtg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tpqsmtza.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kcbkowai.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rxtxffxh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlvwrvyw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dhikbzua.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2osjzgmxi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rjdcaizx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hsmuetkg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dgslvajo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zxbjjgjs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tlmiqwan.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ovzyqepm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ygilwzqv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pmgomzma.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2miuflorm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dvzhwnxy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ziruiinw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbysbudd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2agrnqrzr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qqlzrpmr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2blfduytf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2fczikwwj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2trwznkqa.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2otryzksu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lcggtpcq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gucnlaor.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bxsbhmil.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2soffjmqr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2deykwwvl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ccutvflo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2virlykzc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2schzrnoy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rytrjlot.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qkcpohlv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bimqlcck.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2navflanr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bmrngdov.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lmxfdbsa.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2eenuyyxc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nsksdgje.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zsouhsyo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2abrxvxoc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kbgvhcva.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2krrzkmns.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2drbglfki.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ptcrdaaz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2kuvjvzvv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hpabksjr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wzpvrsff.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2phprkkmq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qlwblkny.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ordwqfkj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qyjvhipg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qmyjblln.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pnjsacbs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cbpnuglx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdnmqnaf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qqgtxynl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2srvxhayx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rvjfdfmv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2kxfcnfvl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2cfgerrko.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tlmbualk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hzrmsdzn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rdxfsnvn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2sdlwzuqm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fqeynvih.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2tnbeleec.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ysfffbii.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wavvbsqp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2svksqdfu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lwbstngw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hxpyjtie.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2etoeguzw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2oxjudlet.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dyqwtkqh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tglwwzep.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2whzvvajk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2isznzmbx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lxroicio.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xpgshgwo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2krwxkepr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2uimrplps.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2sudnlleo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2yqrmtxro.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rdfmxzhu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2spxexhzf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mikrgrxf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yyigrhbm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2obuzjkxt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zbjlsfgq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2aynodqlf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ezfhpssc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ykbhchyt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rsyhlawt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jiqezcpo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ntxrjabg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pbjdkmjw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zmfcgknx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2raltuvxk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qadkdbuu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kutswltx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pukzedqu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mekwbjhx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hxkutjaf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kxvuuumi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dmvludkj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2eqopshms.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mumcwzvs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dnzxmmgg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zlhnupbd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lgyuzogb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mpwkvpew.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dvssywvq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2toadlnow.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qzqiozzo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bnbqwaht.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zxxsmcji.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fadzjbwk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xmigmjec.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2stpgzndf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ezorsmxv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zazdergk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2opybbfoi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bljiwvac.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tbrmahwb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xxlkeqab.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qtdomodk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mtfvkxhf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mxedvzlp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fqzhgtwx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zbhsjrwd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tcemhrzw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vffiwnip.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2stpdihej.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2honaldvj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2pjctlewx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2thdbodlj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yfdagnbv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2lwhdwzzw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fojslsez.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uonvbdhn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xguwoarj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2caaxdmsl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2nejomcwl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2llpnsoka.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bquijebu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2tzumxzig.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2vbttypuo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2hkgjvoqa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tdesxzxs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nqvupmiy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rxbdabbm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2bresymga.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2nhumwxlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxcjpmji.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ngepvwxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypqxghak.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ujdaytox.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lsvwtoru.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ncycrgad.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2alughwim.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ebuyqfyz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qarecmoc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2exeefhyq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lrnfrzqt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ctjfvgkv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jhrlhdbo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ptkbkuba.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ubwpfmdk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2oqpwyfwb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nwvhoahv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hfnmzzgq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zmfxljtq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dupvqwoj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2eyztcdjd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xdqzcwsj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ssgmfnwy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2mdmfpfkp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2udfvamai.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wqrnoijz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wlowimmi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zuihdqcg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ertjifxc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2atjxyuzd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2yepkoxnb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2adgtawna.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bpkstxpx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ecqawdty.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xdzvwlst.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2csgzihuf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yxryadbr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jmznkllo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eozacdzo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2veomstoq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ricyydge.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2yxcrtysd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ihityzxh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yqmngxqc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fjvolria.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cxhroawi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vublmcqn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zwhggxyf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hsvzyhjm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wehevnox.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2oeoapvks.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qjcgsbze.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rhbmugpq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dbdtpmaq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jbfncjmx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hjtcuhgy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bocsefgj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2uongehze.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2nqmyjspf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wakzxdgq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ldejozlh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2enwsfdxb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mfhfmjbp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lxlkmjus.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2mwqjtwwg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2lgazrcgo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eiwpzbwb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2egnwmgkr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ibucxovq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fgmnbhum.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjvvsfco.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2arxtvpnq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zliidabi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cmphxfmc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jxbobbgn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ocxnsoxg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nmrsdtfn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2talxqwjb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2glvaxjsm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2oduoirfd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mevsnstx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2banegqze.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2pfplrfsc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2imrayexd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wvvrzfko.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2uoclazkq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xqcwowhr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dgwgdrkt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zdbdajen.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tljzlgif.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2tkaoqngi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jeiyyyrl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2oifwddet.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bobssivs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uzkwjair.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yaszhtvx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtkzejfi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dvqgbotp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfdlzyuz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wzsghyhz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdnmbvdj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kwihaqep.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yfvtksud.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ruyoqbva.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2whuwjskl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2noijeers.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bbpcylsf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lfeibmln.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2anecfvts.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hguvoulk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tovvcjhk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2lwxlyyht.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mpxuuuoq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgeadeat.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qzfcedcr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2urubhrno.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2sokxccku.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hjpxhcwr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wppquxrg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2bnibcinb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2uwnkequy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2iybtveea.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tkaknuof.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2psbpdsmd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zfxirilh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2elwouzak.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qchpqhyz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rcjapdpv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ilmnwkwz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ohgxfbxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqkaqcmi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fuppavtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iksuiyys.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mfyghbds.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vnroxuel.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2usbdjowy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rqbgrfgb.html


<!-- 参考信息 -->