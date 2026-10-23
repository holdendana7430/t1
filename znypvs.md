代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jneiwtls.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rdvrdbdq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lsrquwte.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mrqmjxro.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dencprex.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jbanethd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3lpbumwxi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lvdawrrp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lhwtdyrj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cdnxqmay.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zrpavxub.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3uxjzanxy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3prvzjiud.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3omtbvicv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3pfvugopz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3oehlhhyl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3migoourb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gbotinxr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ixrjwyog.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3yeueuvdv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3meesdawm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3auisivqr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3svgkalak.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3slkshemy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3glwpnoas.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3znvgbbwq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hlkifbti.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xstauslk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qeshkmqu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pgpltzbw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3lrtwzate.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3npclmjrs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3eclurciv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hlqsobag.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3juusqwbu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qipwgyem.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3reaeapqn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3apoohjda.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3avyulgpj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wlcbgzlf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kvridszn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kwebazcy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rhovzesb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3verdfrtb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rkzlpwaa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtszkell.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mrlrierv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mfryozco.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ztjjfpab.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rmelakqo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vadcdmav.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eknfqgdz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3trkxhmgl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3exoliuhj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dsutzxem.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jfuyhfsi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3scnyqncj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fmukhhjg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3atikrria.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3aytgrehu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3hxezlajw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qmzhuuue.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rkbzntuf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ftidaykx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3owqakjye.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3abtgmakc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3oxwubylr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngyoujcz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vwytchjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wookuylp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3kjholbza.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3kubecjxf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kksxdmso.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nbkweidj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bgklbjsb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxfditiy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3oveslvmc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yuyetlsn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3uqanidhn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ytzemlkh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ebjtpmqt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tuffsuyq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tpylzmoq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3afecwreh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vhfzlvpk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lzevguzd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kovjkqww.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sigrulbi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qsrdepah.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uxlfnrtz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hzqrcttv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xdhhjcbf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wxjxmcug.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wayupaib.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nxzacllu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ndlscnxg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bjzvmumh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xyrfpeus.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zsnzirfc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3aqorheow.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rrhrccbp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3izmydzwd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qdiemqjk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yhrdjmoc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zwhrkzun.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3znuzjhxu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bsgepbnc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3dmxvuduw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ysdbnjhi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3glhxbzzc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pwyebeqv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bykxdmdx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ikkyriim.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3szusfdjz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3czolqmbn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tdczctsh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3arijxnsi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mohrnkif.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3swreysst.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mmkjjjdm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3envlzple.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jefcedsu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3pddujrfe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yssuybhn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pymcpjbi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ssmmmocx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3grjyrwxg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3oawhzghr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3klfiwvyz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3prgexgyv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ojjvppcc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3onnixdfr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qsdtcykj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xqoebmko.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ohiuapvu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sahlamnd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfliksgm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qeiwdzvb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbbdlooj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3irulxvlj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ztqihrdy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3stsvinnj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gxvzmmzy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3khnatdrh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gwpaskks.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xytqroob.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3legxaozu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3apreephx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3oabdkiem.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zecgypia.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vnjjcamo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3aqtxlehe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jjyusixj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gihdtsjm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mckyrgdh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3neuvjgbz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xulhkxmo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lnedvqpq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mssbzmrk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3inlbkcmk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3sjustzmi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bdptucsh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qqfydzno.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rzcapmmd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rayozovy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qavjlvxu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ezekhzyz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3skujqktr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bmifwvgq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3akpgujcs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3spvpzelm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3sxjuvjky.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ahawmryo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ejybjzds.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nwfuwwdx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3owuykqyd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3xmbhboho.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3crwtoyxh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dtwrhixl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3yxbucdnw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3altynlay.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3grsvwenw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rxafbuvo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3resoxudx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ajqlurna.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yrtwojcx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3suttwcps.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fzxynvdi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vnshrkbb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbytawff.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mgfetzmz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yzfcggvw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tndxxcej.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3defslbng.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3uwqwjols.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yvdfuzaq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ubjkvjpb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcuqztwr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3wswujgth.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nrnhtebq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3isuanqpm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3smkbhkuq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bmbcwxca.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3nxoghtun.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rvzidhyj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uphpmxee.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3cdmiwmte.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qcvktvyc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dzfwojqs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3prkejpsq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iyhwgyxq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tozokwwr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gdphdbgu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gdjmpdkb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rfkbgeeo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3crjjwjyl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dnulljuw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3bbpsnyfp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wtecemjs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3idloabzz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ororyjxz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lhnexgmq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ukhyrufb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mswjhgum.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vstmjvmf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxsvzhwe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mlahkquc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dojsxyep.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3glhynzgo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hsitdmra.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kscswmkz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3uzyojxit.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3aujclzfd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3pwtzabep.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xlfwyifv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zelesovw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pxzhfvlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvvwgpfg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3svshdbcn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3iucbkexq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tihreexr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wmjkvitw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ymtxdjbo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ddeeekdc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cnruncag.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hbnktasq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hicpbvcj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dicrjyqd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3irdnervq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vhwcxieh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3otdkvizl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ncpjprqs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xljbmaue.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3knzcxtwo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ygzyhoax.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3wkdtgvcm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mpkaihwz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ooqsszle.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uvnqeihx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mojbzpfm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wacqmwok.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3oibhhkkl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nefckclf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pemuwoqh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nybmcnqs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fvimbsuv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3nxnzxsye.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3latjbgim.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dzzrpbha.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yzpujyvt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mzspjlat.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yrqocqys.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dluezjld.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mkguevru.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dhssijwh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3shhfcgnp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wkwgzbte.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3optntdvs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3scsqedyx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rpviaepc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gybvtlvn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bwicoyjr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rtluhzng.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zgosfotn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nskscseb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ywphcuxm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mwimjjsy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ofkdxbel.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3arfodvqm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hxtcmsfu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xsbohgml.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3oarsbhxj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fgiknyxe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vhffgweb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tkkrdbva.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fbuaogrp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xuewrbji.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ueqkhiew.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qhihvklv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3exbxdlcg.html


<!-- 参考信息 -->