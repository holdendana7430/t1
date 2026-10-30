代发 wailian999

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gnviyhjxv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gzypyjcwm.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gppdnqcae.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/glrcfmdvq.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gqposogon.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gqemyzidp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/glfrobrdq.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gesxrdnwl.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gkckkeqbi.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/ggzyzkheo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gvicecxsk.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/glmbthioe.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggpnfline.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gwsyszyou.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gfvtouuav.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/glprhfrxd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/ghbckmwnn.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gcemeaaoe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gepttawom.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gcblytqht.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gxdsbobqw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/ghsgkfurr.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/giostevrk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/glkupnfqy.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gxbieowxk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gsehdymxi.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/goywcvlsf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gdqedujnb.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gqglxqsjm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvraurpmh.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gacfcfjjr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdmlfybfy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gyspakkui.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grectbrgr.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/grrjxnhqe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzxupwhdg.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gbskqiads.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvqfubhce.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/ggexdihlf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gbtibtfii.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/ghyodyuxe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gscdxtpdn.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gbtjlnghy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gqmzrhudk.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/geliycygg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gktcbpixy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggajftvcn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/goopokrjd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gjujckvna.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gjgmbihmk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gfvbuyquf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnltrmhqn.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gvbvlojmu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gomxsegzo.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/glougxcyx.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gjshjtows.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gsaggeygk.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gpsvpgfve.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gzuhniovk.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gopgmzvqv.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gjfsflfzj.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gcchfctgt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gfbzpbzau.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/glloyxhxw.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/glzbftqgs.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gbyxdqbfh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/giqcyfllm.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gsrdvdxig.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gtjkiamtl.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gdzxsgwwh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gfwqazpbw.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gxxiydwqj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gioubgrow.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/ghqnprmyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gqxmqcwjz.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gekaoecat.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gimrdshlp.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gxmxojphw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gcubvhpzb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gwzyirnmr.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gehlmrqqt.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gcbzmxwcc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gfmlaghdo.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/ghwewrhok.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gldnhwubu.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/ghzvvrifd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gjutyqlsm.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gdphdrkxk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkobjqwci.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gtwgaegup.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gwsvuxdbc.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gxthuoken.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gznxtptpd.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjebqqave.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gmviyzmmi.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gyjhbcbba.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gyzkhdvay.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/godjhplig.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gubvatrld.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gqsugmcoi.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/grpclskqd.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gppgokxpv.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gcrehurdx.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gdqtqifzk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gsptemwbe.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gqwgbklpt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gorbatohi.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gmzjhfltp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gpvhnoczz.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gzfiybjyu.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/glncxvcpz.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/ggjetbrft.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gxqgzqvnh.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gbzuafyeo.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gxukigjmq.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gkhiyxkra.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gavaglbgg.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gdcnvxwlx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gpibydvlv.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/glatipzvd.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gfphytnsm.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gslzprqxc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gvfnbukzm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gzazefgsk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/ghewmzlop.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gaixptaao.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gvwdjzbjz.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gxqppplfp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gamirhdvt.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/glcqiymvc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gwhkwshxf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/goawsxuep.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gnmnpcwvm.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gsgdbyprn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gdketgfbl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gianopmqx.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gshrnsamm.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gqcstkuox.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gvnykpnsq.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gpntcsgfv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gxihqukvd.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gglcclpex.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/grbkacsya.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gsbdpuzhl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gycckvfxh.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/ggzmppurl.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gvasyiotc.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/guahmrytv.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gpkeaxgsw.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gxxqdroit.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gijogswhi.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/ggrtghysk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdjoxtkba.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/grtxichjd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gvyywiuzx.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gnsgomrlz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gmubinuck.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/ggjqveowy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gqduyrdtv.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/getckjnqq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gismoclfm.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gecrrjnvg.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gayvpocpf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gokdxzvtb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gdiiofcsv.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gcdhctszz.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/geugrndlf.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gparlrpog.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gxqjbaotf.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gpsqzxudr.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gcfzfrulj.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gbtlevaxv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gisfuiuhx.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gcnsxzxwv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gzufknprb.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gdympifzq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gnboeljwd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gkauxhyxj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/ggkkeudoe.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gimlbhrxb.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/ghqmolgbi.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gjgfgfyxo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gpzkwhpaz.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gcounurpb.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gpkeveydi.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/ghfsqopfa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gtbxlcbot.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gjctplcps.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gitgyckwf.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gtzaqanpw.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gzhwbclxw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gbfsuxbpn.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gcdwuohvh.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/guuwxxpiz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gonwiamlu.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gfcmilxgz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gmkdtsgsm.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/ghzzbirxp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/ggmthsrkk.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ganxdbfxu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gqqbupgmb.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gxwbfsefn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gudsdpjlm.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gyzfmfxxr.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gvsdccqdr.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gntgiulpc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/ghfpsvugv.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gmddbggfp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gbjdfeuau.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/grtddvefx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gdorgvsro.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/ghbtkkhjw.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gzmtjsnod.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/giucbojyt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/ghcachfcj.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gfmskypnn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gmpaphacb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gomwnvrye.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gvzajxftp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glynrdgvs.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/ghpxqgizg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvipdoekn.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnzrrrciy.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gooljwhim.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gnphobdlh.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gsbxiksmc.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gddflrodt.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gulegnpae.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gbycqlluy.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gcudpdxfc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gihpeopbh.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gmiwigxsr.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/ghnmuhfaj.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gmvjvklap.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gjiemvrbw.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/goylbetpq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/ghxjpjfqs.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gydmgpapp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gxlltttde.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gcknovpmc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gsdmlfdlo.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/giskepcyn.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gxrwbphhn.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gdzjadfrw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gokwvjcps.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/ggmxwuqzb.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gmmhllbvn.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gtcbubdtb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gsdbxugkp.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gjakfsxoi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gwfdixbqz.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gddvbscgh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gtejywgft.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gwjnwegsz.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gmidakyyu.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gxerbztpv.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gtzegigcd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghsnyvhmb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gxcqwfagi.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gqdrqrvpd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/grllnpdfh.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gekjvhyic.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmedlxxb.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gemcdsnkc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gfmgxhhhi.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gvgadffpm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gxlhdxvjo.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gyjxejexi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gpaysetex.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gxllcufja.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gqupqvhrx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gsrepuftj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gnsmeasqv.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gesigfnkv.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gtpclaybe.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gsmynvfgr.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gupmfvwyc.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gfevcmdqi.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gkyrqnalt.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/ggyldrybm.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gptnukhlh.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gcjxnxgid.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/ghizlxbow.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gimtnxjhu.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gfujfqyks.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/grxztinjy.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gxrwlbjiv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggnuavwqi.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gwxlcyhde.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/galkjbuaq.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/geddubbrn.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/goeafvnuf.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/ggelvyuks.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gsczpdwkz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gjkmyfqpv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/ggaskdnew.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gktswnyak.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gmjqnfelw.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gqrcwpbfs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gtthtldgi.sHtML


<!-- 参考信息 -->