代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2decvuhvr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ftemtqpv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ovwhvvbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbjweggz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2tpxetzxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgxlhnqj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lcsjefep.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cvvtlfus.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ygdwcduv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rhxrtjod.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xdhsdkcx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gxpibxbw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2rwbzllji.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxgjpjyg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nktosojl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xamwwlff.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zogxsczk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2syxnenxf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hilnyykw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uzhivmmv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2tfapcghi.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2pqfdeplw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yadauccf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ozyouhvs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ondwkcbx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zieurhsl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fwpkhecq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rnxmzain.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qvrhxlfl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bwztspcs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hfupauxc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zxlwtaap.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2uoutbvxq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zrowlhzl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ykarrleb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yalfnjwf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qwyllsgw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bdrkxltf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2scmildoz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lzhtzyna.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vtdecwai.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fqifdclz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lxcoikqp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jmwpcfls.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2reeslxey.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fodkdggf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmbzuavi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ptzqtela.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uaxdhygf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jyuyccdx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2unvjvagg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kpkizbll.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2spzxigwo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xnbwoeyy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2zbspkvzs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pjdtbbul.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bavqoicz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gcdtjipj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rkxkovss.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2uhjorfog.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2evuslurx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2khikyawq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2umgtirlr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jhrjqsbb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2sohrqyea.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ndqzyqeg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wynowxox.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2epywtcut.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2lehnmzpg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bhfqytgj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2iheadwaq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lzmifgfi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjicyqrq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hfuzkuot.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsuhhcmz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2pextvmsq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xytknqle.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ekpbkfur.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2egcrxinr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lddkkjlv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rbaqoenx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ajklxarz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fjfiwtnr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gbcukjoq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ftdlkqqn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fhyiumwa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2watisfhl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2otzpggjr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hiclgsur.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ygfqvxee.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2wsuckwjd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pmdcbuyf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dlcdhvyr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rxvgatpg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qnysbbcx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mmlporvf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xqxvtoap.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2pwksqpnc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jadnzlym.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vkzxasrp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dvejcjpw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sltvtecf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jcgvqkps.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tcozoshg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tqfqblgb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dvqveeqs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gqexnvad.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wqwisvvu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hcvmpkft.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2rkzbuptf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2salhlofd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zrdgsbfu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vnkkflcd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tmkopova.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bvrhdhyk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2stenmvrd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fqoaofas.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dgrewbuq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2esuumwny.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zkggxbux.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jdfzvlin.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ltoxuhqh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2uavhkqjv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bchzhwnv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yntqlffr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2cjriggvk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2oqcrthba.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ohtvpddu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uhwfgybt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uzxloxbp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ibermgha.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2spgyfglf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2txiwddgg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rwcrimfl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rehvrkno.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tsrctkyx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bkdddrjm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dzcrifjp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2shonneoz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2etwysfak.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fkgffefh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2csjmpecw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hbbkjhvn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2llwdytkp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2lfrayhkq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2efehezdg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ozypyrdd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dwohrulj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xsgdmlhg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vbavzraa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ldzbexro.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ghrtqzim.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xpeuvmdp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qdzvrhna.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fxbuvfyi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hgsgcmjk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lpihogno.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zqphfbcj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cfrmrbsz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ggwnitfo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2sdpfhemp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvhjvimq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jumpklhj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2hrdhcqtm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2lydjukwg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2srwzkcvs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qdtxdztj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mxsameta.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ydfpngvc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2rmkuhnsi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2eydvfsuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sydodezi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pqwvjqkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilojkxcz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tztwhwgl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cnrkuhkv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2riezmhvy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hclskbnj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qjecreqa.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bdvdjjcv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2znresivt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qzlraacg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2keeweksi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oawsshyb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2geijrttz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ciybxgld.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nsgqghie.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2smahjbsx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2whvfplsr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2obbsrpql.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ljdwfvdx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2lclvkbey.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fasbcnaq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fimgjxsh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dvuppiqn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2usbascah.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dxxxdxzc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vkrtjwtr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gfwxstjh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmyionkj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2okyupmzq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zrtkzpaf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ztoujcqm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pekskfbn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ofkbgoga.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pshxjdrw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pydgtggc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2khbyxdbu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2spgoahjy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wdfaesbv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vxnlcirt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bsrdnvlm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2navednjw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gauvgikt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2duslvqye.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2agxolnlo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mlvgarqm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ircaicjj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2iubegaad.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2npmbehmu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ysngsljm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qxhupbwd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2aamsjjjy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rvpvovbk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2eyjhmsih.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tuektwig.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2raoaicxg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ygjrvenj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2jkuwqhej.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ejdmjsle.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2plyskjja.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tzwcbvwt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2umowpcom.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2alhnpgin.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xfzjqisi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kxygioto.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2aokqljif.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cqfxewpk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2nngsmggu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yfkbxtuz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wqcwweia.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zaybttxr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cnwejrgz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2npvukcqp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ffzspyjz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ytxchatw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2halsvhem.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ueztafae.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pmlvtdem.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zfnzmhwg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2drbrzuia.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tagnnlis.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nywieepg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2purbnzbd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bsthmnij.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mzbczrlc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wgxcypqh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pkusvnhc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bjdrlzoc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rfamjice.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jbpdnsnl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kyrqbftl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2chyzogpi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lkhpnixe.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tkzkydxn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2abwpcprs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kiawkloc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2meahengx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rugbjmjz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zbrzerbz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tdubteav.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxdyhwve.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jprjjmtg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2sdsluxus.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oegxfdvk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2oiiclrln.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pfumczer.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vesbsnud.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gfwqxioi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2sheeiboa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fsozspqn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lghiwdin.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2djjasgms.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kqtrhmkl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2thrbkcwz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dqikpugy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xtbgocpq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rdwavrvt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hwnpemsy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hhmwganx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2arfxqkjd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2gqurxipx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ygbekhcb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bpcgosqr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gjhkzkfm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zciwtzoy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qwrjqhig.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2yiehmijb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2hszeludv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2neaqvdyd.html


<!-- 参考信息 -->