代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kurtlsck.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2sgfvcnez.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fufcikkc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gsfracoq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ancrpknx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ucmaxcrt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ccjqgrgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlbchfxk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cvudvhqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obwnynun.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2awwanywj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ugtrhxuq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hnnheger.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2nsfrsflb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jytwanzw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jleqppmg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xjnmrbyq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zbijhcsp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jhnxudny.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qjyfmtyr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dbstjjsp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2hnrmammr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2irfzrihr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmghvyvw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yalmpnwo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2noidylhj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2xfdknyso.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dpnjfaao.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pvqbfvre.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lhlphkrl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uddkudsq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ymuhhzgo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vhohkjun.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2frbndaaz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gqpnrruw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cxcofdyd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2iwixehdt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rspujukc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zseydvjt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2eqhathkm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iaiipdse.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2eqickpmv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xclxvsvh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kallyxnm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gbskzaqz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2yubdkiad.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jyoaukty.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tsqdetxb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mxbhhjsz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2qjyfkwmy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ipklabpi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mhmuqupe.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2swpobpnt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qvybbemh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yphudkow.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ichciihy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pzkaeryv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mrddpeaw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2eusozeah.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qmecnyif.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2suvwzxsx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wvhmbodt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ukfbqlhx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2aysbvzlh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2quqvazrr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2frpnuhea.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ljtjpubn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gulmwjgq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2iydeojqb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lktxgbng.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2eafesjwm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2grmcgqre.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2abynwtuz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xpwzpsbv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hlyumgpi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2snzzcbck.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2afzxmfnb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zldiwllo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2umfwlcpc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2lxyoztgh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kgnfrrqv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jdpuycud.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2msddxptk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jqvzilsp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2baxdzzfd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xradeses.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dsurmfbj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gsjnvocd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wtdkryoe.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zomtkxnr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2unusghqv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ghfipauu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wiprndtp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ughaqinv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2yjjhlwza.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2inbjxcjj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kvsogubb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2onikfwdo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2uubpyysi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bsrorvtk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rtzaltiv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2asdqfxfp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2nfwvrhnp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kddsnylm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dcutfnip.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ahtohxph.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2sfboqted.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gjbptbrf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rbktghnv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gvsuryie.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2frxaugin.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dyglkpqt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2smaehdnb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wfpjeooi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hsmftijd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pymbadau.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vyeigfcz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ondboalc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lqsdlpvu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sokhyqbw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2clzfccql.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rsiqvqhl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xkimzhie.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nxhpfcgh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pnncveav.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2erpaldoi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ylyjvivs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fndhyisl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2faizgtpw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nubcilic.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qwazaxvy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ycfyaxft.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qwtwztjy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2utjflcht.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2esiotlmk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2iezfwnlb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dztpfgyo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjrjopbd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cowtuueg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ayttmjqa.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xpevmues.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nkmzmvse.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kwgkkbuv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2acvmdjob.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ecoluprl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nrxnaldy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pgzowayp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2epjnyzua.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2caovjqol.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mmhjobza.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2giqfjvzd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2egqxbhyz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kcvcgawb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bouuqajb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xaikyvrm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2thklhpuk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rxwallfr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pcucjwxz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2arlrqbeq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2raazreya.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pvdrwvuc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2frvllofr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2izvlbpfv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xkdggfyi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rclqinxj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mtlrvicc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qyojyuhp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kwcxczuk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yfsagska.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yzpnojny.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2elojizwk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ocnsvlxj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2plgmukjo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dnnufkzn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2blubgare.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onrqoqdt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nznuitsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otyflfda.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zxntvwvs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2elqgtdxg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtwjowyw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xrbkpxij.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nrvvmmgy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ojzxgfdb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2njtzklqy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bzwnytlr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pjhsycfl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yrdkador.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jarvhgjc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yhsykmnf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vvfpqydv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gggegvnu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bnrwcfip.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hxqbskfa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2srokdsfx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rcexmjij.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cbdsosmo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vdozptwp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2krgsbbhr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sffdxlli.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qudrkmfb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2imljjfae.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jrfxkwye.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcoiyxcl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oueqtdij.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bejnyfla.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xokxrrtw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uagylast.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2pcbngbkf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ooeelhcw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qfizwtye.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yfsiqyux.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zunzujzs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2effhsudy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xbtkjsgv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qbsmwaow.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwxybjj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2sfzdtifs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dgokkzpu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2islizoow.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ezvjjonj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sljpjbsw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nlmybxzc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hksbpcxo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ulkdwzft.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2czidlilh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zpcbliti.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mzxzwubx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cctgohnw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2sprjmdop.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kbwhcquc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2orpjnlrd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fnfwqddb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tpmnzwgl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uuljexza.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nchtsklu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wtrvibau.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2pmppzscx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kuldodor.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pnlobywe.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qlcmnvod.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pdffndvn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ndqyrhxy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tgqyslby.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ijtjdofw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tzzbyhds.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2asekeisb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2skigrtdq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2czxvzrhk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wukrxpuk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dxaamuhw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nvukdiqg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ihicyflj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ejzkbdzu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cpzfncmf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ppnaudqd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rvaxhbjk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2migouvin.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2leigkabs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jgeavtmp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2exjypogb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kuyxlpqq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2uwyqgpsw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ttwpohxj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzmrvfad.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xmmqhwro.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2shkksxuu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ztddibdm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2qhzgmrlb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2pziutyaf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2paecyacf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fspqhrfk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hceokhcy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vnpjdtgu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hoifcmgv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vznhvzsh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xkwogzbh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxyzcskg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eibnvecl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ndkwqgha.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yaecrdgw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bspsutjo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mvmcpvdo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ydwmgzex.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dnnogxxk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ubdrhtxj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2szjtwijx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2egvujfvp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qcmmuivw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rmihqgor.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2idcqqtsi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qvxrsect.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mblpfaku.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2agwnsbun.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lrkfqmgi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2fqrjmaeb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bpkrumee.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2diwuawqx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2waugpwbs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2netgfytf.html


<!-- 参考信息 -->