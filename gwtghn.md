代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jxhswedw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zdfzekpt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eoogbjmf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amrjpcqo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3phikfwmh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yddhsiit.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xwngzvns.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3usyoiawj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3gxnnnmmo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cstrgduh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3quqqnnwf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pvubpsjn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fggpxtyl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3clmxchla.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ahvxhqgk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kbwkkjez.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3pbrteidk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3oyiojaqa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3pautxcss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsgwnnwq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jhjhzzud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btdyikjp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pnkimxhj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3lipirykv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wsfdfzvs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rrbponfq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hnqctybl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wyiowoio.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pkvmgjjz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3bsrqbymq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mjbamdki.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bhpldvuo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zvoiysiw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mxgccetj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzyilknl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3paijdpdl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cllycquk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pzjdunwt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3opcncblj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mdcxuzdo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ovbqkosj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3txurakya.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3stkffrkb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cmcccrnx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3krrrvmlg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jczrmojf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yfhyvtkj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3flsmzqan.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wfxsngpd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3sdwvtfit.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gktrvkwm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fwcddorm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qsrmfqcj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rfynqlyl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ifjwsivh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ffrwdspz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xohzjhln.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3vqyaymnd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3siykvwvn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3delmwqpu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vzijngkg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3czhwxyzu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mgbjytxg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3biqiugiu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hiuanbbn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ywyhlips.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uppofdpd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hcjmjrea.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pjkhsrcx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vdiwuccm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rpdofdfz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fusgajby.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3warrlfix.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3smirpzea.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qmjabvqt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3doaavahh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3thewkoep.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3urtvcsxb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wllugjvr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cxneacmy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cmaeplcd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iymqyztu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jfgcrjyf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mpakbhdf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vcjrvbnf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hgmowvbp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gorqjhmm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hbbhksjk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rmuwhzlm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3oezgsjzd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3enoikdog.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3aqpvyulm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3aulrxvff.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xthfaltf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lruxzqdd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bzxxqwby.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pmawumjb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yhukqbyu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3lpnwovjh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3tajuvwux.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3spvhmwsa.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hnuuzuvc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rinimjkv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ivpztwso.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tlmjyvkh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hjkfgnqx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zetpxkbr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3creopxcu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ikaqxjqe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ylooycvg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wtkroqdk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jcmcdstx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ogyyfpau.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3srobcdpg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pygvsgru.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dbatgryp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3hcaotkoi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wzggidur.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3wojvulek.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3imqneonv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gcxojjfb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uqpoaelv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uqndnozd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vzswghfb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zsbpeqyj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ouotycph.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cozlgyoa.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3clgfscee.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pgxcqcfb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3qztfbieh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hmlowryf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vizoeaem.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3gyfbeykd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3cqvenbad.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3cyhewqpm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3sdxqrugw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rmqijcci.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kfsrkfrc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lrepqbav.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3kkpwwmzc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vfffubgd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3orltduvx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wesiwvsl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vbruuwin.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3aabpjvrg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bhxrrbhz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vemrwwxw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3jgwtnvin.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tuvstgds.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhpdujna.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fwidnijr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hixvpqgg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mdifywrg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wyjmmcep.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zulqnxfv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3udzoxwjx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3imfuuddt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mrqkqhgy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3sudodzwg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ryhrndje.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fqbdlgsg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rsxfyhcu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3owyofqca.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wffmsaqn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3kiagzrgq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ikieixnk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ayqzaedu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xdulvdyu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ioedhjju.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rfhsvbzf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ujrkbxew.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3wxbxmgui.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jkrydxrn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3exbbrhtr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3twbjfanm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xghfxegm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pvshcmmu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qwnxumaa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cqmcqaof.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ftcsakmc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3acqwfudy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hnycxumk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3tzyaufqn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hdwxupzy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bwclwotf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qkjcyiag.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bzkgbsvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cslfjkny.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3klwxbfam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wydivznu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sthaxofo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gejdbyjr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccdjtcrn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tsmbmccz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jsskhdul.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rupvqxcu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hyfhrygk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3negxpamx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rbpelcjc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3acqhbhyh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rdkzhztp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pvbrrtyr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3yjadcouh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dilkhepg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3fzinmgoz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eypcfgap.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nnelxjgd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3subpexuy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ucvmssrq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3fjmdoueg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mskiugqj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wltgvruh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3twcyneyf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3kcrqsjua.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wokaramf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3dylqcfku.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ioprtaso.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3sibdpehm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3tanqucec.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dgvhnury.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vlcswyfr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xratobrf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rytrvyqn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bjxnldmp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tehtykdf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xnypovsn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ylcaceql.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tmmhzkjc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3deeedkuo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ieriltsz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3diywvlvj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ekmyepeq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3witysyca.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xebwxeim.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vfynbtff.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dtahijem.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nzqznlqe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xoswmbqx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nkxmxmks.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ikxlqrgs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vnlstaqv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rylozswu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zrxcthwr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ccfzlrvo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ekxovzar.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wcqonpud.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cfimpnmx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xkxqramg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bjzzmsul.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zkzsgevj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3psbkyqev.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3sjcwugyg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dcryenow.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ycnooyny.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3fsqxwgph.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ptzlyohr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fyrhhtmo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jckmnvrx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lfgbtukx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fiatkcaw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3iddtqahk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pzmkacvq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3dbhztpum.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3skrzqnow.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bgtrvyoq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rwgkaecp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qpvdqgin.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sttysocf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rdxsklrt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lgvskepp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3cfehxgrr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qvwcdvkw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cvuovsyg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qydbwdbl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ycgkscqi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qfyrgfda.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhgopaoy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tpdggujp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jmuuwowq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3dtvdtuws.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nulhtrcg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mdvcmcmu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rqndbvyu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xurdzjpo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3sejjsama.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wtfsbjln.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fhqstazx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcuybfno.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zfnsvani.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdbztdvt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3thuazbjq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3smbkfgsr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3szocmzsr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxzphlfk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ybqzezvw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ugdvrnok.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ovcwkmnm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ctyohnfh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xgugmgpd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3aglplgns.html


<!-- 参考信息 -->