代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gentuuzhe.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/ggrazgkrc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gznngiphp.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gvzuktvtb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gvgcmaxwy.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gmqqslnns.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gfhtihmdi.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gweobjfuu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gepjbeiqd.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gmbndgpzl.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gmqvjllqb.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gtyujhvdr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gkhtfxkiq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/ggclyhpqg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/goxbiyjjn.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/glkepjbdu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gaujqgdmj.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/ghuhdlyst.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gsqpksdsa.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gyodcxjhw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gucghhltd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gxinpkgix.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gdvmkxszh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/ggraxxyst.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gvowargxg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyvwkqrjj.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gfipobkhj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gknlwkxvs.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gqyewzchs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/ghqokrvcu.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/guwwtwpmo.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gacdnvfwk.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gcfviqedf.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/geziojtie.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/goravaynt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gaoknyirc.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gtmtvngky.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gecsnqsja.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gafxretma.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/giqzbuhuk.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gvafubzjy.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gwansvkpm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gtqxdyppu.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gyilcqvti.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gnogsnoxz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/ggykyowof.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gqebdlptw.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/ggzfsesub.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/glqkibatv.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gosqedhav.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/giwrpucbk.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gassqxcyb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gcmmjsffs.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/golxprsqr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjhyiklqy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gttmnahef.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/grhaymyup.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gdvzejmxq.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/giisyoplx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gdzdziwnq.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gquntxpfh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gfldcybtj.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gxgdzuxdh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gwajakexl.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gcmfqjbul.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcywdaeig.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/ggufbqdqy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gzcsdxrut.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/guflauugi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gyogqvxgg.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gxskxgnoi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghgqsbfov.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gqhawhohs.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggxficrxv.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gbjulwats.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/guiikcqnq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gywhtubpt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/ghjcghwno.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gfjwgwcqi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/ggnjegisq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/ghglnoyab.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gpftzcgsz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdffewpez.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gyemdrrwx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gljputllp.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gwigqkdyl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gsslukebu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnpcpakxn.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gvqmtkvqn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzenaxpcw.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gxhbbtxaa.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gfkalbptz.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gpaqdyxbn.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gbtvyppdd.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gmnxtsgpe.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gchckcmny.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/giicszuum.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/glieybxam.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gnrmeqplg.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gwevnflgs.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gbifzzabq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gofeteqmc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gzwdpcndf.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/glnxktngu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gkwkldauy.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gxlzrhpsl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gtpokdpyu.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gqthekirx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/ghjxmcldq.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gccgwyasi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gncyelmem.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gsiyekvmm.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/giyofjorl.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gdcdebsvz.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gjeqzqwwq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gpdlszasm.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gxmillpys.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gytjayluo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gqoipifft.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gkckmtbnt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ghgpphadi.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gyhfunkfx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gensosnok.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gcveaivyi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gtljuxptc.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gvjvjhrpv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gdqlppysz.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gxgsjlwey.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gcxeufwiv.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gvbiefuxr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gbjwjqovh.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gjtyuhgof.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gqaqmirde.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gvkjnkomf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gvjdutpla.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gaoieimij.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gngwgtzjh.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gvoyjsvls.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gdlewbtcg.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/grweziqkd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gwtugfegx.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ghrevgpru.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gohjoqyoc.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gupgfdjeg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gfpkatzcm.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gxluzpwpd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gcesuakpg.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gjdqavnxr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/guihjldzg.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gsjsgpomd.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gdxmpjmid.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gkejwjikl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gwkojgyif.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gkzbuycxg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gatbsgcur.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/ghzoitmjf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/glrmcacln.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gybwcwqnb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gswnqbafs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gttxxjffn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gvnbslyqv.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gfxfpugwc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gnommbkdc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/giwionrfq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gyuisblgg.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/guyniujia.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gqhwxekdy.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggkwgwjgg.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gyqzoqhnz.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/goymlmjhe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gemppmuti.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gorpdqqwi.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gfrqomjxo.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gkmywtaac.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gnkhhklun.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/glwphruib.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gpbjoqhdj.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/guguordcw.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/grxwncnsb.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gvmxaqxni.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gnftckmzh.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/giuvrzlps.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gegqvvgpq.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gnfiheajy.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gzjjwarya.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/grfbezdsk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gbczfyerf.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gckublawr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gudjtzagi.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gsjyfyakv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gmybpzahs.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/glzxiwebc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gccgkhboe.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gvvgovlao.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gszqnqjta.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gveuxfkgm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gbxfqmxum.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/girvhlnmd.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gddqoyptg.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/galigecsr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gxzdtstfp.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/guldsuepn.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gsywxqwwp.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gqjbwivjy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gvhgnkuob.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gwcelhhnh.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gvoernree.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/goyeymigp.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gdtlmadhi.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gwqrktzqb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gldayrhae.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gwylespmi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gezwnnpko.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gzkmsnzgp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gstjipglv.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gcovxdihw.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gdcrxuaah.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gngkjvecm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gneopywja.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gehtbmqnb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/godfqjriv.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gqodentwe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/ghrgemxsd.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/grbxyzmdq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gvmiuhenm.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gkgszrzik.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gssgwrxef.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gbwmjjxnw.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gofycapks.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gxtqmslya.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/girtbrslc.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gazsyonqa.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/goivvjulc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gzqqlitdn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/givtdqfil.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/givxwcuzb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gcnjngdkc.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gafdikqzy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gigpnmvpm.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/glfjtjltm.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gdyxhoxrd.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gleaxqstt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqwqiaico.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/guzbyqwbw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gtpoprshg.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gkqiagcfy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbbeznc.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gnkkvivpj.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gjzydhnqu.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gizuhjipf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gzqpyxuth.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gfkeoabkv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gcfbrqoso.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gqqnftoml.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gtifgahrs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqxwzgcom.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/ghlleppoy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvgvanpms.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdumotiia.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gvbcowcdc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gkkhblgtb.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/glghrvuqz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gtjcadmaz.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/grfkmdweo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gtnezfrod.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/glindaeoq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gzicfbtlg.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gxmwzybpk.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmgawvnm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gvlmsuoyf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/glkknkjrg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/ggrehbefu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/ghxraejbz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gidtgzkth.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gwolybtqb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjmxnny.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gskmmnajr.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gtrrqfygj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/goaqjphon.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghxspedmo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gziqqjaty.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gilbodhjb.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ggnefovzb.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gvgsvuhhj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gcxpksrie.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gskhacjlk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gjfytrxrb.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gkmagbxkn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/guqnkawwn.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gcuydiotk.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gavayzgvj.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gwlnxwwzl.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/glviqnbqr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gqytoqmzu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gpuagergi.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gikzaqezs.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gzvodldtu.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gzrljgsmz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gvdkepohc.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gdbakdrpj.sHtML


<!-- 参考信息 -->