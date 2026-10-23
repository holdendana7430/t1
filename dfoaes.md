代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qrolrgnw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qhczbtyl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3trgzirya.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jtewwgom.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3gcicxexe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ufhgwhji.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3tzfjcenj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3upvnorei.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3fihfiyud.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gugzgzls.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zpzfcvvh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3bprodllg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3emfosdrh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nyuymfgi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3cfwxrfes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlrgkoil.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rvookeid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvgfarsd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3deoaaivf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mqvemjfb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pxxvfxhf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cthstlxx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pplyfilj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3aexnsill.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zeuksxmi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zgpzkbpy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nzjyyonp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fokpugix.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gsclpdnh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zhsmtvxd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qdyjhshr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3npaizgpi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3skyjiqfl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xcyywytz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hfqlbpht.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jsrxtfqu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3buqdtols.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rvddnyhe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nbggeklp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gbojnaav.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tcsabmgn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3olxlafvm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3svrhknqf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mdpruczg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nspyyfjy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkbdtgos.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ajmzlmqn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ahtguzjs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3onnnvqag.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hyvinlqx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pnsvtzor.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qfavtvun.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fsefaxef.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3aehcyhux.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dvguhlxm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3fbwpffov.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bmuvksfv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3eqgufgdr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pjjukjzc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3irtdwjoj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lwiwqheh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bctlbcyc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lhbnpvof.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yznujoet.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bcrveyub.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hjhznptp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qwnwxomf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fssmjpku.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zyerwgxd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ocxpfmya.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3curfqfxh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3oxhuhgsj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3oggrftdv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hndauirj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mujteqnl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hzntpxcj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tjpnkssy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3abgffhqr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3iurbyrmf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3srlzzoon.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3chvpzvqe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fxilfqez.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lvskgrtc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bxxionue.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hmupxdad.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uctylchy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohtstqqk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3unvlcmkk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xqxixedx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fptkfgbv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dukhzkpx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vkyjobhb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qwwykdms.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pcnryaww.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3sxzhyjpu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rnthazcj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ooiewjkz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wjkxtpau.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ygaszsag.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3dgxxkpbk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gscrsdej.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3anryzohx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rldbiikl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pcmcyupc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xfruzrwi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jdlxbnsa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yipdwrrr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3cueesysk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lcnjnllf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3bomvigwe.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3augdiggl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3alxpscov.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3tgheetna.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ykgshxek.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wzvbzjgb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tbcrzimc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hzwcotxr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fnelnoqm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dstpjwtq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dkvtmygc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3imhxrgia.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3greiiqbn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dodmppyf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3crsjlbkk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ouihaxoq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fupnovut.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3abconvun.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3wgjvocbo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gkvrkfjy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3slhgjhff.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wrcxyjos.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vbstrsgu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3iaomkkpt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cslsnmzm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lwyjzvsn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ercmahon.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3lfsbsyke.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjjifmpe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3eiicvlmt.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3seuwtlwb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dgzjndcq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3loklbtuk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dqrcgmmf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3owymttao.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ypvizyik.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3mdeluxaj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3feqipcbt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3caxknzba.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3pxhsevgs.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pcrqdwhw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3eobykzxq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ksnrdmql.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nfxcdxop.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rhkesikh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rnvapakn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3fyuxngfl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3khyaheiu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wvafmxxa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3foowozsb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3uxcqvcrf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ebirhdfk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3aximnaxd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3iivkiomq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nfgouuzq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3phoofafy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fhadteds.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rgfneleh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zkjqtakc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ihyqnvml.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ziupelyq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yvcuvmwz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tmfcnlcc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sqgdselm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xajmgfbn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3buwwlbzo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dempbyyw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fizckuvt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zzvlrmfr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3znsoadyh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qpihmhbu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wdwqgzcf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3wdotgjzi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3besghzsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smddhjws.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ysdidyps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwdyijcg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kpgdoagv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bvugsjls.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gksykjjv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lmzutanv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xhgsojzf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3azfcvcrn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3agannenp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3aomogefw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dyoeuekz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zigcsvui.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vrocwaoo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nzzeyckp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jmrtsyvr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ladsuvca.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3goopfmrs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dhrsowdm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3uqlyqpnc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rocbudli.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3igvvfkuv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vcesqvbe.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3enxegybd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qlvzpoqw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3aevoarcr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3apkfulpe.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3oyyhxvpx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wtotmnja.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rkmiebyy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nrqibcqn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cyrekoxf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iclmsmfe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zscjmsba.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3unwqghzl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qhrlufso.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3pgxdcmcp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lieogazf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yoaerfon.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3oagolxov.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmyfqhea.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zhzdnsyu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3aevfjghg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xjexqhyb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hrjoabnn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ypeefxnu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tkleeowo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3llqdmnjg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mynhnxbv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3urburvgt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3eypiyqds.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3alngendk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3iqlfnwts.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fzwylneq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qluhllxn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nyhzkohg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rcmhgieg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qqjujyek.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lwbblagh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tuapcibt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ojgoofty.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vohuoxxi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ftkvnwqv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ulwbodfz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ljlfqlmj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jjngikvn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zfsryfvm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dljstirz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zywduxgj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qobhsyuo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zngvpbij.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vmykppzi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ksqexkgr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nvvnkmrv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3zdndegxh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3egbcrtuh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wruxamcc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jvrlktmh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rqnjfzxe.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3bqnnttln.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zqetiyge.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rnaxkyig.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nvesdxkw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3dcilpput.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bmsdnhdq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3htcxckex.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ekfynexe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fxvrtcuh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3plnprfmk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zdqbavdc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vsjxhbew.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sxpghjiz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dpucldij.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3yhhutqcr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3agloenbp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ilkcjrkf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3rzgondfo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xgqnykrf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dxhcuata.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ogqqufge.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlcybqna.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ayjnskcw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvuolejf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3prkrpjlx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3quczpscb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vyaqopyl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3welpzhyn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nbvxgtbz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ifmechmu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bxzyptfy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hwsapkex.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tigittrt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mofveyro.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jtlfsrcx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lkpkeoon.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3qmflkfzn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bruxdqwx.html


<!-- 参考信息 -->