代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qpizyjar.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqgsnaom.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3erhpbyjf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jwomgnou.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qoajifvy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3hwiteqrw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3qnqfqztw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3riryrbub.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3soalsdbh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rjitvseo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nxogopbi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3tqpdxzuo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ccpueswu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3slxdepii.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dpahsudj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptmfyybx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mkkdcrqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpcltwxw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xdacrvmy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3irxodrad.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jteppbto.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qyvbckch.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3miklqxjm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mqzpbunz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gukoyrbf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3knmunekm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hdtxyzlg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mkhcpvzm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3iderlovk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kyautsho.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgbldjzz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxvpooyj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rfgpmoci.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qjakipdl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ckkfgjjd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3falxcfte.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vkkymiok.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ypzvrauf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3fezhdlyt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ipcercuk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tducyuyq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fjezzeza.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rrsprkgs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lescsbie.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pdklujtp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfkxokfk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3igfjdwsp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3laawztie.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3akjxjxsn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ravcupgy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xixgfpal.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oylqbnrs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3omtbdhyl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3obhfyslt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pbcrxixu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vwvwvwqd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3shjakyjc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3fawkmliq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nfxadfes.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3peqbulyz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqdjbmhh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3pfejmjcm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pvcxctsj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tyuleveq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ndowdqhj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3coehybwi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3afdkyqdf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wjspqlky.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tkfbjpyd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ttqtnhax.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3yjksbphm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ecexoppf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3clsyfznj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mianqfcu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qqkmbyff.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3urlqlmcy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xptgmqrc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vgpogqmm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xviuardd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3elhhxkbo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jmxjegyq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3esqpdczg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3nuasfjlr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ltakzznu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzhtiuue.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cdgssgts.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jhmpflgt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3jkzzvdua.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bhlhgmzi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cradnlqf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3knoyvvdc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3urkchuxf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3sfyfvcdx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uxlwvowx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qkwjlyoh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vsegqovh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eohxufph.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fxcifumc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dpuzhrwl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3evcqecni.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wcpxflpu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3badhwbqa.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qahjxxyb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zixocrop.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yncvrltf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3cshbfhvt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axsaniro.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aercsyjw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gjgghzzh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3dteushrc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mqavsrfd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qjsrfnls.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nuzodgfn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3esmusdbx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3myvhbllr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3unryijmb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3itlfgjmn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3shqdgvkd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ygtmygvm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gvgoewof.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rhbfehlg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3imimbcaj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oefslyqc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qzgvqgdv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fumjsnuv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gcbilxjf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ddzqztvl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hrditwih.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nhecjdjc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ehlswsxz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3metwxkzh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ukwfpbmx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qsnpiybd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ttchuaxt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qswqxbaz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wzxyqkea.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pbrrcbfo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3idsjlqyi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cgigdldi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jnklwtly.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rzflmhdv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yspdgenq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jtwsbwtv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3heilptin.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lesgvtya.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vxrmwbgl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jbhmguhs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hqtjdnzb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dfojqzri.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ahdauood.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dgprteqt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ulympyhm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3frbgjjfo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eppnimwn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xycezhoj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3svkxadjy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lgeetslz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wckzbmwj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qhruznvm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vbolzzsm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ktafvbny.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rllefswk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ulqejztf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aehrhost.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3axhvifxi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wognjxzw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nqqzigov.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wrwckulu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ayksbbca.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cevvlvyq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fnjmwmaw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rkmkxnfz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3acezssao.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3icxjgfhe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gqmaybpx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3epfqbsak.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gkeandhj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3prgxubfl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xvmicahj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3cwbzjylp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tkrupwhd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pjhwwohx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ylcsotay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gebiwvaa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pvicesdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbgfdxdg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3amhziocw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3njhkwysk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zlmgkahi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dzmxupwr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kzmretjy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mkmyoznz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3laqypuiu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zfmqpmfj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lfvcugij.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zkutolfm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sedqzsyr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hrdmgnim.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3djbdisjv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3eiqqyhob.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qoeimvgd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dtycfknt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pujjrhgo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dlhtilwp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3itqujoyt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ltarbsqf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3eesztaec.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3twcpjuon.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3trkjcsbx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vehurhyk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nelaufsq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3aludzcof.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qgckjbhn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tgcfskmc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dtezjvhw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gekgpmtq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3injszngp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mbxdjyuq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rhmzrbmj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gpvmmfqu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tykgufww.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gofcllvu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cehifocb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gvfierko.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hobtiygi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lyizjdtw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jguxltxn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xqgsjxuu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fxsqifkr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fekdlyag.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dwmwxfea.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fnmckeqd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3pqykpoge.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3croeerqp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lsketcde.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vstcswpy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3rhutgzld.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ntnhtdab.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xurhtuff.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3oftxkqsj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3amdgwctv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3sestwduh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3auezvbuc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pkxckubs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3hbckhddx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnqwadyc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yetetife.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3uwxbwhad.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hsdowhgp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fcmzllpm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3sbaddqze.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kxihihdj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rmjktkit.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kekowgyi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ykkwhdoq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ddhnaawt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3eoirnyfm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rwhvdkku.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3neunbxwn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjdkshdl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3pdnoohxa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ecunlxnl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xwbarptu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ampqhugq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3oaxtntkr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3smdcsaib.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mwmslmek.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cqrckjwt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vvavadcz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wwbimtxh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xxrduxkc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3yuktuqpz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zopsbqzs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3abwqzqkh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3fzxhhuxr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lnbhhshn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dwgckvxk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nlbxqeon.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3eopvwcgk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3pgwlpqdt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mxalzmal.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3djajywlv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ownanhud.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyghzwdy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dltvkcvd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hfoxhcmo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pjzlueuz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qpzrhppv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3htpmkwxy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jiztexmq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zkemedic.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tvaujjhd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iagjbrcy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3izxoelrj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bjkcrvdk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3loqkfcbq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ajyxtkfi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nrnwvuci.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lknhrobu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qpetljiw.html


<!-- 参考信息 -->