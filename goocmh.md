代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3yfyxkcor.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zqbblrax.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3flnztora.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hnekpygt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ggssfndr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rxreohci.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lqohfmsk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3sqvnmihv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ktzzgfau.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3xvftcews.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fyapamze.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xbnrfqbo.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zjtzujrc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ppcwrkps.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3flhbvxev.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ywlafwwx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ytpjqvoo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3fnulaetd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ayjarnmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkvswhzf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3adoqrptk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxuaqllg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3mwfxmqxw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3trpksxti.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xrhwaazf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3olznkcdl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wospndoa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rqptxrow.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3japyxgjl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3hbwqgpnt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3kfabkafc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3edngpjav.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mszqqwcj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3epmnyowo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsabrnkw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tsmbalmr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rvbkccpe.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uuesflzn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dxxnyzpp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3udlturle.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bndaagqq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3cpxpavwp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rkzuptur.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qtcilbgl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3topgkdxp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3cafdngln.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ocwvkxdv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zaasxbix.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qovlgtbd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hleiygof.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ahpgtyxa.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3soevgedn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xuzxngzw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hrpclici.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qkugzjbw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3niingtrv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hovvjrcb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ppgzocic.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ciwmcfyh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3arlsksrz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bxervdzb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vnupyshd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gkcgorsh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3welxqrhd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3orrktcap.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3yoolgpjq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jjgzyaqu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3edfwjeze.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3cnxlgual.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hcydnwud.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3hqaqeuez.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ukkwmggz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tyjqfhsr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ishoheks.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3udznfwnh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qnqkfuuc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dzrykyxm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3sgkgtquq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3upiouooy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jdemssav.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3txoewpxo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3uvwaizxc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3apztrrwa.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jcrzhaof.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3oxogfgyj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wuxhuiar.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rkgwcthc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zcjdtiah.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eitqcksb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3okvvugjf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsaccipy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3admffjkk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fdngpkde.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3maviatbb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qyifscab.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3dvzybgin.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3upugbkny.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fmxlmjly.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3brsgtqqp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hzhljbsy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjjifhl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qbxnhbgk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vcrkktkr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3emxcsbow.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rfzmiqel.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lqfrlbez.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hrzxmgxv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xqchgoqe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dqvkhneh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mnujemqr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3rhfcwljd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3efcnummm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xjdtyvbx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3woecpynx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tvxflmks.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3sjhrpfqm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tzuavhio.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zwjnqhvq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3culjhnbd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3drwasgcm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lygdzafw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bwtdoqih.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cbzslpkh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jsdjasok.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dzxnovim.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kfmvclgr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dbtmyfob.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3dipafnly.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3sjgvqpvu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3whkgnqxl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3laiyqogk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ewgwmbao.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3flwvjaxj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yvnfipkx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dvliawcw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jqkmywhb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lhmzwwvm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3mtdmofzy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dvhyhbov.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3efqggvux.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zvygbpej.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3uizhsjzo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mdhxxsvx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vmalftcu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kcuxcmub.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kcabtxpd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3txvweyqv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xwgrzcth.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gcxvxlwz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ntiriujc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sftgruqm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3axcipowm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mtdzvemb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bcqtegnp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dwrzpjwd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3prvgzgmq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3jjmqmmro.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fembbdss.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hbrtidqr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wnxvfoqv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fjiyrawm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nrvsubjl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bxauwakm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ezkxxagd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3dbasgkrt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kjoheblw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3coqgqulv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3chbgipmd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3awkpjocx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3eqcrelpi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3goplllrb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3cmagsdxy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rzzcfbaf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ywwrnmrq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ncdsbivn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vokhbyrt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3uzypsfau.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3swtchicp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3miihlxna.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3tlstpusf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jbghjcml.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ljsbrwer.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3zkiikdpb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vvqmcldy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3yyyjjhqu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xclrsmhv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3iwkovoil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jagyygai.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3whyizrhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghjalcnk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uzdbypdw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nlgjvbfz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3koaieunc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zyivdfmo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wfkffehm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3psmrooak.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jiuoxarj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tyqwzydi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wnacdjji.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3veymltjc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3byviuikf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qywxjrup.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nkmaqyjm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zwjvjnka.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3muyafdmp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rnkbnqqh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3iylwzzux.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gsiqkcre.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3swtmlgjx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zwbmgikn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rmuhfcle.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3svcewicg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ejftjjqm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3czqosbdg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zyvwbojr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rdkjczlz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sbzudymc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kdbkaqwv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ecgclbvj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xtrymacs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fadyoavt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nbvmefmy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fwqepmpe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mzpxqvjy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gwtpiood.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wtbmhpxo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ekmubofe.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hgvjxuxq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wydnfqbj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3aasqxnbl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sxwasmhr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3isixobqs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jermcicf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3moripotv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3parxtnna.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ewaxhpez.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ewmigtmt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ibzswdio.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3penqbaym.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pwoklitf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rfdrwnmy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3irdohwad.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xfosrpzz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tbcujxps.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3oeuveugq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xsexazar.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cqrjghle.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nvzbxlpk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wylrefoo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3txjdooqa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bhkoxxpr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bauxurcu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nmqediiz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zyseimus.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gpjfvvtg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xdtkuwaz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dfdswxxl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kqlbtycu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jsdsmdhj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3wemznqzj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nufrxxfh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qyumosqp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jgcglxfm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3miuxspho.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bgfwgdfs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rvbxzecr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xqdfvyqu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ohklozdd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fwggtylj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ldkjzzjg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zdaricye.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bewsgdkb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tecckppr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qmlaarkm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3imbiwwcd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kudzcrvv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjbkkdnh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uweyoixf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jwflajpn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3scvizuql.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nsjpyhso.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rxqrpgdv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lusivxnr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xukbpihp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3draoahxw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3waqvobfk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uzxaqinp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zutcxevs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tyvwuszk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wrwrjnpi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfqrkxih.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kbmpejsf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dspvfqug.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3wxicrfpb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rnotparo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tmkujybw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3obeutrki.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wxmdatrw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fbbxhxgc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rxquukwi.html


<!-- 参考信息 -->