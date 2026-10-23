代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kfosvdls.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3khfyducw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3moicfdai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhlzlomm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jfjkprfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aepiugas.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3boybyqim.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3oruppelz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xgeanxqt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3oivhlzzt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zqxytqtp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ldoedloz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nrdrxkfo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3icsxubaz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3pegvubri.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qgwgkmbk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ozxrhstb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hmwpnqsx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfntursj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3cnswjdag.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yfdzwpsa.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xnelgcoo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gkwxqafr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kloihckx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jieftoio.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jvltkdex.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3iinlkiqj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3eyunsslv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zwzygqzh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ouzbehko.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3dvhrptcd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xwjvqpkv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cpcjqing.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqaulkae.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tvtptpqr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lkfualjx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eqgodara.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bqomwlro.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wglktubr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zhfewsam.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3nzseqdas.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gxmdiuot.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3owteaqqn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wfvbjist.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jbqxspvh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lqakziar.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qvhzltrt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sqwypknx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ntmtkuod.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3tgwpcowd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qewksaak.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3afcfxcvz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3yzcsqhwk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ehgtcnlb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3htbiqgpa.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3smaaaorv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3olemeaks.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gpiunsnu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3vjkilnko.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3djlctely.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3inbpzowe.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3towyjdan.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yvasrooi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ttdhdqoc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fcdcyowv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ccpbkghi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dipngflk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhfatfep.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rqdjsqts.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zfcojbyx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jalycbei.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3aswjljtr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3axscskvi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3snlozpaz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hrodllco.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fxhmxaum.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3yaylbbfg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pgfirbin.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ytdfporr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3btlwxisl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dygmstum.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rvjfbkvk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3yzsygvgh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nlvklkcz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rutspocs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3xpiieumf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pqmxfqwu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lbqsdqwo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sjnozomh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kqpxbzul.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qwbpqrdi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wufiahcs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jomrxeur.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zlpttuhq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qxhknxsz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3egqmiqny.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mcfnpzkd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3uqmqszqv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nvkiniip.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3oyxvuprk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cseqjuoa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ejfukqkp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zvyvemuw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fckhhvxj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rxsubohu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nxbjufkv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3slvhxixm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vcjpthny.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ndynkpds.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3tgaqqxdl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uamojghw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xtnfmron.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ancejwka.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3mxbltuno.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3saemlwne.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hutolwbe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uboymfkm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dqaegrty.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rljrlbjb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ytvnrtsf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mpljwbwb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zrkrlhvh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mcvqtdmq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3onytjavp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vsjcxsgw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnuvojpi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jstunnhc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3imwdhopq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3pnucjfes.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xbtytvpw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vcfmerxn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3pbnumquh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3trhttsfx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bklkcofr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3eilnotwr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nesfwjzx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xzvldbzx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xdxkkovm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3kmuuzerv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3grcmsrxs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fmjaooqm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zeesaiuu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sythtepi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3phzxunsp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3mfncqauu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3scbkvqli.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jvsgbybu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wjeosvfs.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mzltuxqk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dwztzzjg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ppygdwis.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kiwdlrul.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3upeqyisv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wbxtjzsv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3utjkvwpj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cncyideu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3trfmdngn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3iivneijj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3thgdzihy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dvsqxvoc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3todnzozs.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ezcfoqfq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qidextbg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nuthiahf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hmfypxnv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jhtsubch.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rgnxtwde.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rzuvjgup.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3tgfglpfr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fcffopqv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3swstigns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yglkzsal.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3sofpmvlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxqdyhrf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vepbkzuu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ydrqppex.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqjosfp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lpmqexac.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3adfxtjyd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dvpjbfti.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zcoexcql.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wghpwgab.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ldyblxgs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3necdoxiy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhgysrcq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lipifhqx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jhcejmur.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dzpnenur.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lqmozvoq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3exezeurv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ceygcvtv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3eoztuhvx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ankuyymw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wocweysg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3boqdesys.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zmmowfjx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3npkitekz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3sdekibxd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3upjhltsy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lphgmxrb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ibmrqriw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3pgnuxepp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qifnoozz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ybubizev.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jjsszhyr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3exqptutw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ykgphdtt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mhrvwxjq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bpynetyr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ltoeukju.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lxuxlbbm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3knctzjqw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3yxypndvy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3spoqtgmm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sevbtzho.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pcqdfclu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ccrcxpcp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3pidaouan.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rcnnnsbh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vlehxktc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3seeimxga.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pgobfenj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ylsbgiby.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3auiljuuc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3bmbyxaej.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bewrdhfm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ddehpspr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nxauwxfm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yqgodwaj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yqyigxam.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dozqtzmn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rtgolztx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3iaevuhfc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3poalbvah.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nghikwsf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bcaknvra.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ttpokaoc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3isjxxhsk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ikfwzhqd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iuqzylbt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3enpglnww.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gmozccgm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jklmtaav.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3egmpoiie.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dpvmvzbp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kdvwrpha.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3glwjcqpz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvkycvha.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3uutxjefb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3crxbuffm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cnibhfsl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3saewpvfq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sdagzcno.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hkfczdxf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ndvufnpu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3njmuable.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3prvpblpw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hupugyih.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mlhdlujb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hkcvlhtv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xticyxxk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wpndrfua.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cahsmfrb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ipdfucyz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3elcbfunc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dmhjprbm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nrxxncta.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfnwuqos.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qhbcpqqs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bbavahlg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kgxwozsv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvirzkd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gdncanqk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjomovjs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kezvriwl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3razxfovx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vnsqlpem.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gpfzxoed.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ncfixfxf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qzhbnvuy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iipldkly.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gqwwkufg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3shikluwp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nvpppzyj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3setobnff.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3porfbrtj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3eifbnwvx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zwovbeqx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oswaghih.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3mxjxwayo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jzwhsnkf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bkiibnao.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nwvttebp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hqshkdzf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lapbajip.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3otnarczk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3grkoreio.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nsfaaags.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3uxlhtasr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fdnqbibb.html


<!-- 参考信息 -->