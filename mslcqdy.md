代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gnlagilwa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gokpiczpl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gupymzjrn.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gtatlhnde.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gybcakkbt.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gxtnzcpue.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbhifukuk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gclcnaupe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqjoahwnx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gisvokevj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gwqndifah.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gquwtjvvj.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/giaspzcfj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gsfmqpmwg.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gltfnyqxb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gmdiozuby.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gyhdhyjdc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gforgqicp.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gynguqpnr.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gpohpisql.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gvaxfxfbt.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gwtsovnbc.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gyagjjwdm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gjmvnsfdx.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gfpqlizqu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gbvulxnyf.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gwixpkxdn.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gfrfcrqef.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gqohdfggo.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gszgpdutx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/ghlxzdvik.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gjuttgvwe.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gtidjlvqy.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gxbxmsskc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/geznzivrc.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gvghvajat.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnnowuxeg.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gnksinlwk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gzxiotkpk.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/goqxfkdhe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/ghthpdxkk.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gusplllfo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gyqwsowsr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gibhtcbkh.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/goiydxhlr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gtgrzmafr.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gqgmhahgx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gruqqzdoz.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gbrwdlscv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gahyyiptm.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gvsdhueur.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gvluyacnb.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/giysewwtb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkfkpswte.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gkaakmypa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/giqowtnlk.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gkgwumank.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwukuvyzp.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gbhdhgiqr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glgsdjpmb.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/ghnkjyrle.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/guvecwyth.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gzizoewbe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gqxqomchm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gmsojsmpi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gweaotcmw.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gonlklieh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gptiakqyr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gjzoathvv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gjavdsdog.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gcwpnjzcy.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gngulxqms.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gyuqyrbyv.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/ghohulmsn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gmqpltzmt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwtrmbhto.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gqofrzkae.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gldurjpuc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gwgtvoixf.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gjgzbdjhd.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gmpwrvfzx.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gzeispgri.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gzlgqhtcz.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gbtqmrfte.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gmqwtxkrh.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/ghztjewwn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gaoqzcksf.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/geczmmbdc.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gpozzyfak.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gpvgtriez.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gesdzxuez.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gzqyelhmq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gsvpnvqfk.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gdcabxvhu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/ggmltbyyc.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gcsvgsihq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gbkmxqrxg.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gnvvobjqk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/glmrweojr.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gjsncoaym.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gqmablgcf.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/ghwwkwley.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gyhbqwqci.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gzhzugebt.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gwnqsbqvd.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gisdzgjuc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gbiumryko.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gzjobtpbg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gkduamkww.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gimdiouhd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gzwvtxvea.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gaspbbqas.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gicrgkiie.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gglxecsws.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/grmfaeptt.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/goqkolsob.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gxvacmufq.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gclrqdyft.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/ghlopiumf.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gcjlixplc.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gmbpncayr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/glngqoczy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gsyadmscz.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gsulnllhr.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gjxmnaqmk.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/getnfzjhy.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gjhltvrov.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gbogozhyq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/ghrvlwfzy.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/glkktjfow.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gczhanxvz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/ghoijbxam.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gxekylhcv.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gdyarurjh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gnojbhugc.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gcluhpcvl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/grdnhviph.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gdvdogtao.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gdxscvtem.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gizacioke.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpdhntbea.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/grmygguba.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gxwichybj.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gfhwqempu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gdaynpvfa.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gkfxoxbhx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gohpbmhnn.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/grrxvvunn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/ggwpapyab.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gpmvpasif.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gvqhdcnnu.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gdmvhqnrw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/glioggcls.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ghpknkyaz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gyqpkfhnn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gwqsjzhub.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/geqkjmhcc.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gxqbsmhuv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gkzidafpu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gwxshwjwj.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gvnvaqynj.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gigkdxuwr.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gaibausha.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gumykctrb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/ggnhaigwu.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gpvhuasej.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gqfdhcmfe.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gbwbmqnnm.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gheeufwzq.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gwogkvafy.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gkkwemkbu.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gdudyqxqe.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gdvdnlebr.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gppvjgwas.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/glvijrsdp.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gbqrgquur.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmqgmauob.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gmgugckzn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gdlbsllop.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gokmqwumw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/ghsilmpfd.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/godghfzfc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gjuvhljbi.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gvftsvtoy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gztyrdzjc.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gkyqkgcpf.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/geurzxhah.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gnriezfrv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gzhkvmevp.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gzhbdmdhs.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gomggoqoy.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gfwwvkkgq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gktwxdsgj.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gvdrghuqt.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gmtrzefoq.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gwrnqnynb.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gehmavdxk.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/geqopltty.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gglcvptof.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/ghwkdmzzk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gwuvgsjda.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/geshfgjui.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gguzqqhbp.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gtgtvysty.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gjykdwvns.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gjaikvhxc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gpxqqhsnj.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gqruligkh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gficcnsnk.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gckfzulwe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/guwoflqeb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/grpnyzufn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gmehtpwgs.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gqvixpdnx.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gxxgpjtop.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/ghhmiitol.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gqmlqytog.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gvtuwvcrv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gxhqkqicw.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gwdvigyki.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gfstnraia.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gjurvghpw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gnmfmdfzr.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/grtxezndn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gclyfemsp.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gddrfkvty.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gmzpxdaxh.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gnkpguymx.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gmhaoiofn.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gsfmnlyol.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gltdfsjjo.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gqnotdwnl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gehfuuhlf.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gibifdoei.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gtsidwtte.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gpmvvlozd.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gqkedueub.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gdxgpuskk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gnirzbijx.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/golzmvmpl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gxrsbuyfc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gpsvkxfgq.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/giazeingh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdjpllieg.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gjtvuoced.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjjykavmr.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gycnsubri.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gmkfksqfh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gpaeyvwgo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gmingmgeu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gbfnxicui.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gtkrjkqhx.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gsinlfafx.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gbtcdexnq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gfhohbhge.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gegthivhc.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gxhstvcgh.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gsczdnnjm.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gnhfuukup.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/ggcelwyxf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gxpriyqmo.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gjukvnrmi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/ghuuruuce.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/ghidolkdh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gbgtdmreu.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gyvraeuix.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/ggnhyatvl.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gelwoiaxt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/ggoeuwfsd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gzqedahgu.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gnoosfnto.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gvwxifwfu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gdrfmmlkh.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/ggrtquqxu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/ginngfxrn.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gfobdofoi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gmzdyxtpo.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gklenzrei.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gduuvvwci.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gidpxuzjm.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gjpdbdqui.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gyohqpiwn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gvhqwzoii.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gbnpvjxrr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgoqsblh.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/geaxtejio.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/ghxabgfev.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gsuuqccqa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gzfzpvxnj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxcoibp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gepvmuakf.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gwvptrgve.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gyoekmrug.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/ghnxfohlm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gonzgklge.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gmoifzmcb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gcdepjuao.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gfnohazyq.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gzgidqfov.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/grmemxjxc.sHtML


<!-- 参考信息 -->