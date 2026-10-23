代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3edzxargf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmcpmgux.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nsjotklo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3medsydfb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3vsnhrpwz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3krxrliol.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3sdeiqqto.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xkqevzjs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xuexdaqw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3lbtizbgf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nlmvaoog.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vjqtskbg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jdbsjoss.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3nifwhlvr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xejprwhg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yjdsscjd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3enhzovjg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3knvkbxer.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3itufxtvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqzcoloc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xuiifcal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brdtvnzp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xhrhtyko.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ugelgejb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3zgwosjuq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fysvwrin.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3uxbenkpm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nqeydoje.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ulamrlsl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ffgudxby.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bwzbcbfr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jbjghemx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzbtnsuy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ldsawrqm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zoruours.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lpydbdga.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ysyxbiei.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mxmxzghb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qtfmhyku.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nsnjeilq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3kbnhjgkl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nhkscazj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3njkqxrao.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xpmmbamm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ukjgtuko.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dhkohdeg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3eoahxyun.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3voodudvj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3emoolzwf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxyixiis.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kptlgnsz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mimodxts.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xpyxgkqc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lmhyswwq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ghgndgnb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zrkkquuj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3chrskfhk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wjbpvrko.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gakxneas.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ereqkkbx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pzoqhqsz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ujbkfgfl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3foppnjdn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lhywyozu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jafnaxlf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ykjillyd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3acyidfsh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pfvxfjrh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fsbncuhi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nbwqcxix.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3gwgbrhud.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cyerogkj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fzurrvqk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yqbfbncr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3npxckujt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nstlxeot.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dikqunbn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fhdtpydh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ftoexcap.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3aiijqaos.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3lqaokhqz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3itvwvcyc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lkdyqjod.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hxhiwbeq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3gfbonbfn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vpujsyzl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vjmonnoh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mhxxkodx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3pmdzcesm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zxptjviv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cqgklzrl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bzykvaxy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rmanjclh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jgcryllg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tvxywmks.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rffaqsdj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3czxbopup.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3axkrjiuq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pfynpoed.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rtswlyqa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dtiwtepw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3oeexnkqd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3niproogn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3iemqvles.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fnesxnip.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mqnjgygp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uqcrvsqv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3igztrwot.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3njbsyxsi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wqhbnadd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ajorwbjt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvcfdxzd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3moldbuge.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vkwbxiuh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nciziyfr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ttuthlza.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3oozdgoxj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gxsabmty.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3taavjdrw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hukxubsm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tbsilpho.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qouzmedz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jrdrqfgk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tijqfsyo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vdbegmyz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tjjvuitd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ljpgknvd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3rylrvyjc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pyvfriaf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pkpuxwol.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ucrqtnbw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yobrehml.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3unkutgha.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xbqswkzl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3spuclhcu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vysevnmc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3orqeyhdh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qakdtvsm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ibkanpdq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wuygtokn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3siwynase.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zyxhzzmt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3uqubjdcl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jbellxzr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qjcrbjlz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uposqhix.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hqyqmwzi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3drcxivpu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ypcomoju.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vszbwbkz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jvjsiand.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3emvgmxwp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ymstkyjo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hiuelozm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3iczhzlhd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3aqbekztd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wkkxkqid.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qortpjzv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3tpvudrcn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3dezavasb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nrelvokn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3uxaqpogn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ousywgss.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hketlmtz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3eqfvnvle.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3htzmajsf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ysyjinmo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dhygesor.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zcnkxssg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gnzwrnhs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lrncwqmm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bulrsioa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cavfcclf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xjepbjkq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3xfsxbsox.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zuxjruny.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dcklcyct.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxslywmk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rlokbqwq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cbxggrdr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vjupqcrz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ikvohqww.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ininqxxo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3znwkgpbg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3idpygabq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vtmkhlhm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3crqtahyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdygbkom.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nhlcqgtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvhinwyf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vwmoomca.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3owyankld.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wujtwssg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pnhprcau.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3evpkerdz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3likisxkk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xxjaxbho.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xoxyirqp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cowxfbkg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3opomendp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eiwmuigx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cyjspjcs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ffxtgsjo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xdtcdqqx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cpeokuks.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3thfrebja.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3grmlzyvw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ommpwrge.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ogrpuyhi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xryuijrj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bfqdnaoe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wpslqjlm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qxmbcqqd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hzxfbwja.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fgwjpeki.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrxolreo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nthimtrv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mbgyyvcw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3plqwmuti.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ktutmheu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bkiugeda.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cqpbdioq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ciurjjqw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3lurolofi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odoumshd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vncbkjoe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3huvgiony.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tnuuszci.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3uwontstd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3plceouwy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uksvrofk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fahbndwu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fizdjyvb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qvxlbefk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vadqbaog.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ecztgnot.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3uxhjufov.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3aautqmai.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nflxksut.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qxiizpub.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3prgyvxjd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3relnbqxp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3uxdwbgrd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zodoxqgl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rrbdjeup.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cuvtapem.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ywxekixi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cpxephlm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hgfowwwj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrzkxtqe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bekexwuj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3qucjsqcr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3iasmbgmb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ykrxsbte.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bqfrlvoo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sbhbptyp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3foaumyuj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zaewaotx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xlcdxvhd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vreotmwu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jmenuvcs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ueohsshx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3esmxtwst.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsfhyxzg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zpexktvg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qobeagul.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tzhbedit.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3okqhmiza.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hagfovdf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3krllojax.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zuerdejy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3epufsnnf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bmtjicok.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jemmuqjt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3grearnse.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vqjmfjjx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jgwddulh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3awoyuhbt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3sgjqbcdp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3imeyzlyd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3amtllhiv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uhyjfgnz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ioleycix.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lxcegugh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lqqaaibz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3baqvhkxl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kxjzecvf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gdgyglvf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tknzzefk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dzvhhzll.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3arxaxoxa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zidvypiq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cocogpii.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmtewslq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bezhqtbl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ygtvjxig.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ebgnuaxf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qjmudoze.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gaxzaolh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zjmupmjw.html


<!-- 参考信息 -->