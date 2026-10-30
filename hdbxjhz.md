代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ggucmxwhh.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gyrxejhek.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gcjosjaes.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/ggibvhuqo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gdyueirqj.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gncekgfgy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/grgcukptz.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/goowvhqig.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gbijuqxqd.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/ghwcijege.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gpxrgrgle.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gdclyrtum.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gokssghaf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gvpfudaui.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gjvkhstjf.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gkunasdbv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcihshxxg.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gtlvxhvxt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gofwhiclh.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gazfrygqs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfnjxucfi.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gxfmgcgjz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gqxayvqga.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gwtopkhhu.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gnxaboujf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjgmiilay.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gsuatzove.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/ggbbhzngb.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gcsrowddh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gllmaubpo.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gkwmdgbgq.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gculcmuah.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gsfdsrvmw.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gdpkitlrk.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gsdwfuzlb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/ghqqlahnq.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gvxmbrkdt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gmcrxramw.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/guulbxmbu.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gwvlszaxh.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/geseyjbkh.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gucdjkhee.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gijxbdmet.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gyzczwehc.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gijasidwo.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/goklmkllb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gndpoxxmi.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gskwmyaxn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghbrgzcwl.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gogqwscyl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gfkebqjlo.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gbxlausun.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/ghikphjsm.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gulkeyyrx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gwyduobaf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gdujrmfzi.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gopzflvza.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gdabrgjsi.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gtckqfxji.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gekrcvuiw.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gxwojysgd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gjlffbuxn.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gvlmazvea.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gvhcqelvm.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gwiknyzqi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gaurjgtkq.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gelqnnuuy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gfdmpbgcm.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gwzrqcmoz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gifmqcdkz.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gfsavsjoo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/goigtvtos.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gvxrhxtyc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyvyflqlc.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gkzrxbqbx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/grmbuetdv.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gsubvepej.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gkorgpdeg.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/grspjceld.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gcmjthfgz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/giycjufyh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gsypeajzo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gljvvyhpk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gzadgdnra.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gqhvqnrsg.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gvypsdtpb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gmvfpftcb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyqtrfrse.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gztysbnza.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkoidbqls.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gsxtayoga.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gcvovcgiz.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gyumguwzf.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gvylbatsd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gppkrhgug.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/giymjnwos.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gjpknphrc.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gyjyaeylz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gfnxbragg.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/ggnaaozkt.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gexezvbkc.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gagojimel.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcsabqnnm.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/geipdxrew.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/ggnjqvylf.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/grrjsmwft.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gsbiajkgt.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/ghoywjges.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbyhjsmkh.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gdpumrmic.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gnrhdizzx.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/goyoxpbqq.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gnoddkloe.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/giwgrxwos.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gemjzclvt.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gyycipdid.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gydydhlxu.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gwdkrpvir.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gepcntojb.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gkrfptwap.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gfmcayhhp.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gfaqisknw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/golnnikpo.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjymviqec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gfcfqehfe.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gucclobkn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gkxqxwwqh.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gfrfcwotu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/genknosdy.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/ggrwqjshn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gkzgubiav.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gaxyuatvy.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gvhxnfqge.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gcyqrygpl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/giucjyprs.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gutheubar.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gllsgnmza.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/ggosnqcvc.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gjcancpxd.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/getrsxdnx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gwdbbwjiy.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gaqexbjde.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gtddyikfl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gdnpvrdba.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gdvgksvic.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gnkpmzqoe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gtqjyoyfv.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gxkvgcorg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gztkophll.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gjpkviyfn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gdlmcntlf.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gpwitkcft.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gnjlpmcwd.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gautpjegr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gjxwyxbfb.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gqrsvwoqj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gwotslzpf.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/ginjripvv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gzwtpandr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gvpqhhxdb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gncdgwgyj.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gafywentz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gbusjrjqb.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/glqeffyyh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/ggemflrke.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gqnzjofmf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/garrtigic.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gwggqwzhy.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsomnrerj.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gfdurgzay.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gaejlisaw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhcecpu.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gmuosdarz.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/grutftsfx.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/glkyansur.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gskakmmea.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gowzalgnz.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gtaqxyfka.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxsjwhsdg.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gxziquhua.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gwdnhcwye.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gjlpoamjj.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/grujkdatd.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/ghahxsjxv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gvrjeflyz.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gycxksxcb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/ghyafnwbf.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/guwetafze.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/goflzdmuh.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gofsvbctg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gpthglkqm.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/grilsasxe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gzptxtvcy.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gsoxztxui.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gogsoiypp.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gecjpscnj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gyvasoojd.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gelemholm.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gfeznzjot.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gliomnrpg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gnphmkcnx.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gipsyoqyw.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/glhgdorox.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gmmpzhzpz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gvuoivxrg.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gmwzajlqp.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/ghzoptyzv.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gmwiqbnuv.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gawmvznqf.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gxivbscut.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gvulllful.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gewerkuxb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gsbfotrtz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gxskltirj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/glgrqguvo.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gsedmxxkg.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gmhlzbgnw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gxglgbcgj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gkwqbhnik.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gegyffkws.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gmdclockz.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gbfwrvogn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gwjvicxrc.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gwjgayewy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gxluhhmfo.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gyousobwb.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/govjcjcho.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/ghyufgtys.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gefsolnvn.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gxqnxbrbr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gqvsaryrj.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gzxdxheho.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gupdtycns.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gcxstcote.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gxebnxodr.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gxmmmrzcm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gxoiyqujx.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gpxatappn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gpgoxcenw.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gopgaltxd.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gcqwjsyap.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gurwpivby.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gkrhzsscy.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gosndnqpj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gbihysqlo.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/grhvoaoeo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gwfefeywn.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gbnbkikni.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gdxkgvjex.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gmohpshjd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gbthskwcx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/ghllafszs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/ggaydbbqh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gipcbiqyq.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gtgyappfd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxjybnyyz.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/goqmdnmld.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpvuybfqw.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gcztoxbmz.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/ghyzpmddy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/grcviqrwy.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gdolijtsf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/geebbeffd.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gvckrjqmf.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/grbeevgpo.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gknjibgbp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gsaxfnmnt.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gkxjnbexm.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvwsvtzee.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gtnzmnenz.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/glepiymhu.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gaucbyfkv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gjoveuxxu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gzofmixzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gdlgkidxt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gczascthj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gneyghypn.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gqsblftqn.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/ggwfsfgrn.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gjumiturl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gqlvaqhup.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gqqgmjspy.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/glekxgfgw.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gbnqicrek.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gvrkbmggz.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gbewfnuox.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gobsybrdk.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ggjfqykxr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gphizhwrg.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gyaluemmb.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gaduqhllu.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gkjwrrvrq.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gwnsnbrvh.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ghqyljicr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gfsawzzty.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gttyjsxos.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gisxdnpza.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gsvzszseb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gxegemblp.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/guwbofrsv.sHtML


<!-- 参考信息 -->