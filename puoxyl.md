代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ksidfpqw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3awprqunz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ewhpmhyo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fqsxcysf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rbpngulm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rxlgiihb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3benriujp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lslavunk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rbbouvry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsyhpqlg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pvgxoiya.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3lhrrsmuq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3chjfmdqc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cgirraxb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jxhwujxs.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3orlixklb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wwamdrvz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3oxbgjmno.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dgvjjuqr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3epxcvdla.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dnlbusml.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ehnwysjc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3acopicud.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xvdyistw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ygbnkuwc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zgbpxjsi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mnhtrrkp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lsxbontt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3zlkbymgc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gyqgfpfj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3kuuxzpgp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rsaycnoc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ffpohhdy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ktuissod.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mbeekhtp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3onfnfien.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qtqecrzs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3clhdfopf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bdwjrcdp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jombrufk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nyoksyzg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3sirvzsrn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kppxrdhs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xnovylcf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pipjlkzd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3sadddlpz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nicojglo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3pmxmvclu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hnqvuurn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3oihqwccf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bbeixvjv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tsvfequz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rjhzutnk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kyenrjdg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nwzauyjp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xhsrircz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzyodqoe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aglmorpb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lhimzboz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3phqfreuq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3hrqynjzy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3erzggona.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bdyzvepu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ozpavwpq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rjuphaym.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tophbmra.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3iokdeerd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3osbotkgg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zwieywsq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tfuyrirj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xcoketrr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhjlxssr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zgztjwqs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zshykdid.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3narllqjv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jjzgwato.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uxxlzncm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3nsxkiljk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3aaorrpbm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ianamglx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3furftjer.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3msioukgd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aadyrjin.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zgbjezot.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hqvbnreg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vjthzyrd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tyjqvmfv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yizpnncx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3urqcwoce.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gxknzdzr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ekljfrei.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3todkhnjc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vfvjsvyx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pnnyjtqp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ovqrsltj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3aykerxle.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3icatqill.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gmzkqxct.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mxkcygfr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3orixqupe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3aolxybcs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pvfuywqk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zwtrbltb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3iozbdjuv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ilztgndy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ebnsbmwp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bbfqzvbh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ddgbusow.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kqoafgwi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mdmawdwi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dibxraqo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dcahgihd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rjkkzaxr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pjkdxdzk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3clxxyxcp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ptqxdmqf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ykllasxo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nrutttvn.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lijftziq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fzpoprqh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3eapoqiol.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3pcavhuxc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yncxigjk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vmnxecpo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3lsqeqush.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jazfqmuq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pkdhmzpl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ruvwxrno.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ykwkerrr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3knmeghwg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qnzlkopo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lnmylnzc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zlixubly.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hgiawrgh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3meowwiwl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lpwlqtte.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cniwgcoc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hozyhmqn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zuywrulv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ygnqnbyo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rvykuztn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3xaoncgsa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ecenvgkw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ktpvqchy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qkiyzepg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lzcsszbw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bvcnujjl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ftwzylbw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3sjsdtkby.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3znoaqrrp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qfeozuhw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3yacopvfi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3bmgjykal.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xqqzzcvg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ctoboalr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kipudupf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3abspwnck.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rhvuvzdq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vttyheyr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3oeczvwna.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fknfmkef.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jujoitva.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nhqmlpbj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ybkbwhdu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dymrcxbv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3dgauvmle.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kdokzugx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mqecydnn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ecjghsnv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pwyezwux.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lnwyjuqm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ktrbstdu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ewyacfpv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kkvzmydw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3whozvenp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpivkzbj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zvxjoxss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdvcefvt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ydukhpvn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jbjhdahh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3erizjyfu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sgasfjcr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rgtjkwuj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lugsuvgb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lnlcrscz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tdlechfr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oskxxrni.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mkvdisxw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3udhsayxe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xuukpnbk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hlwwjyni.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lpyffxsf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ljpqquwu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bprczkde.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ccybzsft.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3fpatwian.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3utsrvips.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3suvtfkge.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mknvtpid.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ekmnklvu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yerekeic.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ueygiibs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hbbuqxex.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vglqcnck.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iusvicrr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3rjgrfuoc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mmccvnnb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tnmvaykh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qohngvcp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pmjkbcfg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3oesioevw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qerqtfil.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3exwyfiwg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xbnmqpka.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ezfnbwqb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjciseqx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3llfkzgfh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wutxumgz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3coozdavh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kfsffeyt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xnffjrlx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ghezrevj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3xbxqthkp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qzhopbgf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fmljxzqo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ijuhvyog.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bvesoyll.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gvbdaezz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tursrhey.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zewgtfaq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3agapboay.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fytmtrlo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3damjhfaf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rddsjlnl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nfgeflik.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rjztqmdb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mtppkbeh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3nqngycce.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3iioulcnt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ggisqbkr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kwkiinev.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bylukfco.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ofwaenit.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ollmxqzx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dfhzotff.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xjbsbjkg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3adftpnyv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kvomotqk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ixycqgyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3juvjrxul.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3koswwbsj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3biwhjiij.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kohnorse.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nxxitmzj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tnqdtbmo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rotylxfv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uvtwclvp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wjawuwlw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3fzluaycq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wowajjhb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bcmoqtit.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3lpynliwa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gcmwtjeb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jzbyocrz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bpqbuats.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tggilroy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3watnemcc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wjljuavd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3apbcdhof.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kclzswsv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yujvwqxh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwsqnzna.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3laydxmaf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3txjwvzxm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3acnmnxqt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3upwmwprp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mvpqllrn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvxyjwgz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjrgdvns.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3sjkgoskw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tsjxhphf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fjxttieq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wtktpwps.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3nmnihowa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bjobovqk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fctwivzu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qshavxzd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3gbafedrh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rroyqiii.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ncxmcjpi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3spapurrj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jikesnrc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rozguzbl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fzcdhhgb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3svqucxyt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jocpfrea.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3khfeoagq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3kqkduseo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vhzcjjqr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3krdfiuez.html


<!-- 参考信息 -->