代发 wailian999

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ulnkmydc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3bjglmqsd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tuxwnmic.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hjkwsdgn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ewehkftt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3pbliabzh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3gahvdayn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ehujtczp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rhahlghr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jgvzadjg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ecxxmick.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dbrkodrk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fvzpvfcx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vpwnsqqd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ymmdrlem.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zfdpxqhu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uyagazga.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3gqjuaqbs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3komdtjac.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3sjwtyaqz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bqbhhiup.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gmjsjjhc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pznmhhkq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3niqegclc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dbbexymy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3etisbqbg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3yuwqtxlw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3glpkkcle.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mpkbnbya.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pndpatrt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3oaqicivd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rzpvjhbl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kgukkrgo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yopvrgav.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qlorkkda.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kaacnrcu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3hdjmonmd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ihytukmj.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qaasnjdn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qhsykgwh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3pkjxqfrs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bzuiedkm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jmbxcrjz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ygyfukko.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hmcjihjd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hsklkmkw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jytdbiyq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fgqmghza.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3knbhwnom.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3gptiyxwi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kcwolemn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qqzunpvh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ydqyrjmh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3grguvwlo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fbwabcsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyzdtgqr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3zrkhpnsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebmbxape.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zdfmjlvy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ocqyenhc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3nudglnoq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fuqvntcd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xkgilfdy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3spcabfrt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yhidtspk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vghszcig.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3dkrjnfia.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wkkanxjd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fzmdqtjx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3joohnofi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mivpnbme.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jnnueqca.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3tjqhzcsm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lowqguao.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3kwpmntpz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3msirzybo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sqtledpa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3byiknqfv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yonaztij.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hljzvqop.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ipihaznw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cqdbhlnk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3btwzoyfk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3znetnwdn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3euaiarab.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xigtvixv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jtkrjopc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pknkhdsh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jcgvbczt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tnmxvhoj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nclbbkua.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3txlktzqe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zzbdwvab.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3pkwnjtif.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yzhciuxk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mlmctrbh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3avzdtgsi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3satxedqk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mgkxwgii.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fuajlhwm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mcnqvhxy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jofedsbl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3avtmzkel.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3polwsfur.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bqqnaasp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nqkeqqgp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3quxmjaqw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3evvajwqa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gdyuvcon.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tbqxunch.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3oabjxezg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kotfqbau.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vrygwjns.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ykrlvrfq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fcmxmild.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cwgbecij.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qfkbzdyl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tyiitcpf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yazydhzf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uczwhboo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3iigzpfmv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3okovjybp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mpyiqnfz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ispqnhwl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3owpmpsao.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3aqivglan.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrqikmbu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ghojqvpn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xjonceud.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3bikyalzp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eywkeuxp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hwfczscd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yzimtawt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hxikwomz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3sthbspyt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3afdsguky.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3asmarnnj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wxgweyhr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3urgnghew.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3gtsnuoaz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3txuleckb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dpuocxaq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3crhxuxpd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cthzdcwb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3olgdhuhq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yjkkrcga.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cdibtjue.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mioiokqk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gsowaqhl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pmxyjanc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lrvgccpl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3orwlqmhv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wworgdkn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nmjkgbtt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3hbxarvsn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3chwgnmqd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yewuwzzm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vfndhljq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qxppybug.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fclnyaul.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3legbksst.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3duefcnxt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hunfyidb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hjglxrov.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kstcagys.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3knpzgqzk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3iqoreoio.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ryozfrey.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3oxtonowt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3pxudlsrx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zrwshhtp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3uafuouto.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qyesqbmh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cfszvvhg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3lxxuogmd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mggfizrq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xmuskaze.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3yytencqu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3exehnclc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fdexervi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3lowvbica.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3onwhycxf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3trgupooe.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3trisdmcb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gtjjmthw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3grmmiqjg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bsplqhzu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qdbgixql.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ndqixhtu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pdkapbxn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gxpllopf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3etujtowk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zmwglsxu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3akaienzb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gkkdfqbg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hymfvdzu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3owkvxlwb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dtsxmqll.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vtlrxnnb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3fkfyastp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ovqaegdr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nezvnuiz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ruesoamb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fwdrqikn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3nulxpvaa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ibbqmndh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qhpkybgb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ucqhjumj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lsurvwoq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mofisrwz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3rxtjycok.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vtcuqsor.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bicezlah.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3kasvmnvx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dollhjcq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3yfbjpskh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3pvhiljhq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rbbtwsyz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kdvhvxhr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3cljgcdhb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gadwhyzj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3trapvhoe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nslrfwiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usbtxcwp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hwmzllur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbzjfamo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fncftkpa.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3enhfzwmh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3buezmoyl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tyoyhgir.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vapciukg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vbfenrhr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3vorxiexf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jqrddqac.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gihsfydy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gswapkdv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbplrwfa.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wfqftlbj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kdkhizmx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bpbtwbte.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3poesxfgl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ogtzdglt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rwfosjqb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qqjitrwl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qgyhtpwa.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qbviawwu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ntsqwkbh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptpyasvp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3avrlxgxf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ovmaxbsb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3esvfodfe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3shyuegvi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3guyffaxp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vquxefxp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wewzqkje.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bejstifj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xpjqeneg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pulkhltt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3aosfccou.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3htqggtsq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3twqzuhkn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdoisorh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hjptzece.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3okvcdcij.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yszuvhrz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zxsawaoi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fqqlbiyn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ogfayrlh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dpfzlwoa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qsinvvef.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3llwnawrv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qlyuhlme.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3eoysutdw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ohojjzcs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rcmhsuqr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vyljcbfx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qyijvhvj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dnlsrqnz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3odhdhhqs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3unewhtzk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rkyqlqfl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lnwbiszl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gzceihnl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3mizfjryn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wpjsipoj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbrwaowp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pgnxvzgd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3pwxzcmqi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dmfyjnyu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3esfhydku.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wtgvfqjo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ghmqfpvk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pzgsquqm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdzfzaob.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nghochzi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3sbkxdkzz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3boqcbgle.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ffwzbczj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3aosiuzer.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qtjsblbs.html


<!-- 参考信息 -->