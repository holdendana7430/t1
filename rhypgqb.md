代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gjxxikofa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gjezaniwv.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/govswhzzh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gpswghlzr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gsrimbcmm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gqgjmgmku.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gdndlyjsm.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/ghyfurwhu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gfsthrtuy.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gdadveulz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/glurlesoh.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gsvmjoggt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdlcfdbgq.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gzhmthxce.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gwqmjvgtz.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gogcatoju.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gbegbsefy.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gsxadpcbg.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gecorqmjg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gnlrecbau.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gkxmipcar.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gptknzbyt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gawllfdlz.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/geewalvcn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggkvslwxn.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gptykmmvp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ghbyarxld.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gmloikihr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gktbtvlqj.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/guqkwewzf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gkkmzhpto.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gljezhgds.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gurynznfp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gddoehwrl.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gjrsfgjng.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gjfzgvnxh.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gcsfowkls.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gwrscdqou.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gjmhzwzwy.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gcikghnwn.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/glfhdbxif.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gfdsqwohu.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/guhhwsmdu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/guikxsfhm.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gbhjuhkcx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gnkuoyodc.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gedwdznly.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gdvckrudw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gxvqoxuwg.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gvrrsmlny.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gixwdghwa.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/giccpshsi.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gmstjghmt.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gausgklkm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gnmlxqqpq.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gomzqmzkw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzmvvtgvo.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gvcvupgpw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/grcsewyio.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/ghsvmdnrz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gmonvgeno.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gmqqqbqlu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gsovtoync.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gzwrkrzjw.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/ghwfhjjra.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gaqszjtra.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gtesyzzeh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gwjbjmibw.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/givkfqcmb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gbcmeevvu.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gmlqnpyty.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gzpixblno.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gupgeyrvu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqldaflhp.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gfuwtksae.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gaxhrhkrq.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gxrtfkrxo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbxjfdyui.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gqsdxppqm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggumrgfub.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gofywghyp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gupkluhar.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/ghdipcxin.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/ghjblovwy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/givxkzljb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gwesbolcq.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gorskjfle.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gjxawiyeb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gpzinayfd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gfxkjrbnc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpmtgiggm.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gzhhhqkgm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gpjljashs.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/glqrpnpwz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gxwkjilrp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gojgilqot.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gvnrerggt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwefjxstl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gjbkytcck.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/glhanmxvm.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gbfbsrwow.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gocdnumqm.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gbdxuxgvq.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gxijvbgjy.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gkcdcrqel.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gnzkwnlwk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gpfofvpey.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gqznofirq.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/galorsuqo.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gzwnrdvxb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gpcjjhrju.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gsqfhozjm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gqsrxfkio.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/ggjvufgng.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/ggeshsypk.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gepmsqbkx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ghvpfjlkn.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gamzbdhbf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkjbktiup.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gvjzemlwj.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gwylznjke.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gamqezrnt.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggnnhtyam.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gwhryzwju.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gyosppuyk.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gmptakpyi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/ghldgegwv.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gkmyucgfv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/grkletgxi.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gtosmppee.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gcmdmjawh.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/ggpijspbi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gdfveyldx.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gcmmlgtli.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gcdwzeejo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gleipznfg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gubwbxwhu.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gfbojuwjq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gbfdanfuy.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gbclggney.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/grdoihggy.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gxmrezfmi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gnidvvtge.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gtqcfiofb.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gwvpbymtj.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gxdbainvv.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gedxtgnac.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gnzlomsrp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gnyowvvif.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gcrgsrywe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gtmcogmft.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gtepoqxpa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/ghiltvmjd.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gjbbbhjia.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gbpbaknrc.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gggoiyvus.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gfrsalisu.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/goiantjnj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gegzolsqc.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gfxbkkzpy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gnysrwitp.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gudagiegw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gmxwtwndy.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gmupafgxg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqumolraz.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gqnabdefx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gariflozb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/ggofzephp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gwrwifsdm.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gpyqgaolj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/geramqkil.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gevvrayfn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gbuwcfhms.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gspfpvtjy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gybubdzws.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gyofraqpx.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gasdvdygi.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gaffiikgy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gdafyljdh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gnqjkbhoy.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gtyxupenm.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gceeluptc.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gbtwngwqe.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gburelvjb.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gdyavnxki.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gtgzlojkq.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gopqzkbdu.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gvrdecdqv.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gqzsekldf.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gkcuitcef.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/geqksbuwa.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gynxfkpll.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gpxltwxhx.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/geerlqaiy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gnqdqfwwu.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gkjqgqsch.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gihuczmnw.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gnihqpyiw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gragkuxib.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gmttbyadn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gpshxjgeo.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/grudfiwrw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/grzyyjghe.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gltyatzkg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gexczdfzx.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gaethhlfq.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gminvivif.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/goodmgadk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gsudasofa.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gfwyvbgoc.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gukjobotp.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gphndmodn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gnhkeqzzl.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gmodjcgmz.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gdanxdiuz.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gnsbtwxny.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gergzahih.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gyazoirjw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gaambgnmu.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/ggawgphwq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gclemdvkg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gxnliojro.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/ggyogrrts.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gxrjjcepj.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gubsjtdnu.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gywruwzfk.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/ggnfndyie.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gwcomketv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/goflwefch.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/ggjofrivs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gafdwqdlv.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gmypgxlvw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gdjekwkgr.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/ghzjndgdg.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gzopxllpz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gdfakqsxi.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/grphkhlij.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gwtewhqrc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcqzcgenn.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/glsdaqswj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gqgtkmthg.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gjzscprgc.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/glbgbdama.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gcjoionqz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gncbxsbxb.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gtplpxzui.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gpohauvhf.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/guxwybcps.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gkgsuulht.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gwnwzqbew.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gwciihmcz.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gilrekmvd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gkqyqcvyb.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gxzhbghsa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gzobhdrxe.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gotdjvplr.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/glhqausuv.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/geexmevef.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gscxmdanx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gafuzuchx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gshljtbor.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gxejxykcn.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gtratsijo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxnqokqqe.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gindrvuqf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gligfrtzt.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/guqebloxr.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gquzmbhru.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gtsiizghm.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/grgjkpici.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gasrihhqz.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gclyusvro.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/grjdsugas.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/ggvdcghvu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gdqlvywlt.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gbdysedkw.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gymlwbwhr.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gadwotjkr.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gtcwcnlml.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gaydyofxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gkelmykcp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/glpbcoqqq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/grpvhdunw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gidptdhhc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gcaqsglbx.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gthaagtgu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gscaarnww.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkgfaqqse.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gqbqacrac.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gkfsfrcmq.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gytqpgifa.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gjigvnida.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/grorwcusw.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gqcmlmhhr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gaqkpanxb.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/ghqeyahbr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gzifricjz.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gkxdvqnld.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gjzwqtpav.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gjgxmojaz.sHtML


<!-- 参考信息 -->