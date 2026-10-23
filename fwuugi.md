代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xvnpzcgb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nciwlwlj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3psxhwqce.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xzdlkmnt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hfvushpx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gpruqyyh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3xpzjcipo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3oxjzfzad.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3onnplshr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3oapriroi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3pmvdxaou.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3pecuqntr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3abxkypor.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qcuveddt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecjkaghb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cilwkocz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jujqcafy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3fsdnnkst.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jehhzwaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnynimsl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ykcqjlcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvjwdlfh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3sbpqymjc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tjtaqcey.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pbzkxqjs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3weifdrrl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zquaxrew.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wfgoiyuo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vqznxurz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xihwyemh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3akikdvqg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ivxiaodt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndbbbrkq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3augiclvu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfylbzuj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mratnalu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pqjgmhmy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3cguuggxn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nmouhice.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wroifyio.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ybglfeoo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fkbujdgc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hvlvflir.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3byxvawjw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gnefkwpx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ymzuutrm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nnqbmwyq.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mfyovhqw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3npxqzjsr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysqlcpui.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hlbyqrzb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wdvfatmb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fglamwky.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xoptyijf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lrqosarh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jkrkiabr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rglfmjzv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3yyisooeh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nunyiooa.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ddmsbjno.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3unlyurli.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hpysxgdj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3kcwrpomw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sjpykhzy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uxdhulyy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3pjmtghzl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3odizrnaf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3voogjhzp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lmsqvnug.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tlpbeflr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3gpzrzqnk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bhcnyqhi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ssifdnjy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iycfnjsy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gyhwjdxz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3sytxepdd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jvbfkjpm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pafpuquf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3darkazgq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lrgflzfa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rxplzehd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3nigqivzx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ajqeigdc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wozstyrw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xdnxxxfp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3znuxwtca.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mpnyeuvd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sktfxonr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uvafsovi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xqohfwnw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ylwwowzp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3hkufpeqh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3kybthoyi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dycwhsvg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mlenkxgz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ghzynmsr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3cqlgyosu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3edcpfapj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tdpmgsho.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yvbesirb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nqyvbsrl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rosvkvjd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3dtoqbcwq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rceynmah.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fsdefkye.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3aytkkxkw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xkadetqy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qyhxljgo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nazkilhe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dfyamtao.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3caqonrce.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlimjebo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pitgxyit.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ttqvgibs.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3xbwzogvv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3msonnwwn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xkablpwg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lkcfgryq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lckgrhmc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rcxzpdfn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nlrgjyth.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wxtrkdqu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sykdgikh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sehjdogr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dgyrlfnu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3yeueglzf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ocnqpuis.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wswtfwgz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3uqmfdbwf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zpunktwo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aiadpang.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3oyhjubgn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cadmspyi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3irojfine.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hbmriqqy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ncpuxsrx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3czhihaig.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gwmruagh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3njatjkeq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hhrhlydy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3djbppjky.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nlgmdwxb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vshodyiq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tmtgqeiz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3zpjioxta.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sgeoabca.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nyluqrma.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cmtvouwv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3oteischr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjhudbhd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3clrwnltk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zlvswkev.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ahlhezcc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3yezdqotj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qbsjjsji.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lpvldjok.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vpidacto.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tczhzohb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3tcvgkqmx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jmfapikd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xcuoyebg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3fcbmxnga.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3nqtngdra.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pubuxvbb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ecblxqpa.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kdgqonqp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zebmlvll.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xxmtqggs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ocfkzzhr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nyvldwdp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vsllqdiw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3tvngulsn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nmfxdepj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vxgtcbii.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3katyyrnv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uyncisoo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jwbiglxm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tfjvvhbn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3izztggcx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lwudhevz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qslkmflw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ltevavbt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3sjfssoxh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kqeobqqa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bwbewujg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3actclwqc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pczbqipb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmmfhsia.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3vstyhngt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcwwugxw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qwbfabzb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fmjcndrp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgxqacqn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zjouephf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ezwzxhth.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tknfmiyk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dbhhpjvh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mxyeezcl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lokktizs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3payhejag.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rhtxchwp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eptbzmwe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fjxuhgzl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xwtnftxp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3okrrsagp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3prmwquqj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fqttbsjk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kfrfdgxg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3quowlvxz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3gxvovfqe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3sjhplsei.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmgmdtvp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vibnimsi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vkrxnnza.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ptclgpbb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3socxunma.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ydgmoowd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3iaaonnrq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3kcuwstch.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xqqycdqx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ufbntmeo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3clllrxiz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mrrgqlfw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vyoywwso.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fnfmqufl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ncqtmdlk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3smanaqjc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eaccktat.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bnmjebuk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wcwejdws.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ylfsdijk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hwagepdy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gjgtbnny.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pfrkowsn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yzscjdzp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fczujjre.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3sjwuwczd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gembbvcc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qefleawh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3npyjxfea.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nybjxwdq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wglqycan.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3itwbmmod.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lbsplfbk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3sdreacfm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hjghncdp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yfygfodq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gaxzgjaa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rrnehsqq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jcuelduw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ecgcxjjx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cypbekyq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yqjeevin.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gqeehyza.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kspumjbw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ujbilrbf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3umfletnp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ckaqywai.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cxrxsbns.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3scfebxen.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vqbynker.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqoscdwh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3lzpagqae.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gpwvvhaz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3efzzuwwk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ferbowyw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3moaenebf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mnqbilnu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3iivttgzn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3oyvcnmpa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lpmkvpzp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kgrykrgo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ivsvxfkf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3onspzspi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dzferiob.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hfnuntpz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ckxgcsqo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3aluzitrr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qlmracth.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3oujtelzs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hxbzhuke.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3klzdnuzb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3qqmjrjcw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yalawisx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wyxkuszb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vuydvzgr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ymrgqzoo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xkhjjffh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gwzvbawk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3elayuowz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dvusmvjj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ucwshgcf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3eweiosiu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3viidyjiq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wbdbdqfd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tiavnnvc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dscnvctp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3iequqssf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3scgbksxm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qtseibxm.html


<!-- 参考信息 -->