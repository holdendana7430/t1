代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvgxgjuq.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxupruhz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/grengugsl.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrjlmxrr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gicqannbg.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/ggozycsxb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gmmzwwwnp.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrjtnlco.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/ghvgxunlf.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gnqhkirbu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gayyklqxj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gukiwhylc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtonqexk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnvxwgqm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/giqqzkjts.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gleocxngn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnayicvd.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndkohmoa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ganfxifeh.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqstbeml.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gebleqtcg.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gqarkptqz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gvhhnsdxp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmkpdqyyn.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gynqyyvgo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/guksobyax.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjjokuou.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcjxdfbu.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gutgmuszu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gvjdzmwxw.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfwdrxdt.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/ghyfrrdvc.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfrzpsohs.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxocwqrzu.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbrdqbzjb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gborsdxbc.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbxjqkik.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjclvevr.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobepszbw.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmidryktz.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfspnfwv.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlhucbde.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gocnqwgau.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnlvpoid.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsrelqqu.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gcgmbyvgd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gvlxmtfwf.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmjffztu.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdbygkrqy.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gveidweib.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfvjhegc.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gfackpeym.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzutiktgt.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/grjkmyzqx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjjpbfph.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gyopavzmr.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/glkupbftm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghellsodm.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gzbyfaytk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggabxcxcb.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyukijpsg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gsojicadm.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwmcxxyi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcochfrk.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gyfskntbn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwephwvn.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvtaexah.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwomcanei.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghvfboocx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwxqoahny.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbchohmhv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdblttevf.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gmchaxlcv.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/giimtvaoz.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjuxdsrk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/glxkehhmk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gksrthrds.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gpnpnkwie.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvogceuaf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gfdpzdiyt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gasorpvxc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcclqtgt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpilpxeml.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gqlvsqezr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gxgrnrdpv.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gegrwsuxy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkpiqqpx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfgjowfx.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfwfzauc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gaituycqk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/goqtflwnt.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyrxfzxx.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gmxdrpmtz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gieorcvdx.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gsptjjeih.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/geqhaljce.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gzayqgxaj.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcturpnuj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxunvcdwa.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gekkfmooi.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbxgtzujo.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gkovsjipj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfysrpyt.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gddqofslw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzmwfodm.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbxzvcof.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grqhylisz.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gekboeknz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/glgxzoksy.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxgjrfsbo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gromckaqr.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjqvkqak.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/guiczcgej.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gymzxosdv.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gltqtpzzl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ghnnnvnmf.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdbxyaxt.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghisrieiv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gevfumwli.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwrjsfkf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuykbgmy.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapdaigsa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscylqjuk.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwzrmkwa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvbqxngq.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gchbyssjh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkvqnmrrw.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/ggdztqwox.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntajdens.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtwobqtp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqwfyloxw.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/goesdbicz.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaijnvqwt.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbljqhhlk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glhnkggxq.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrllrcyn.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxoxqsqi.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhomelza.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtabffpic.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaynuyzq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjwvdpsi.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gydptkikp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxziyzxns.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gentkryrj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxmlxhirc.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gslzsvmvj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gguardvfq.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/ggocvcbiy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxapaaps.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobrugtxi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/giuoliiux.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gepqeqxtb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdzeacni.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gremphyuh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyesfske.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsylnhehg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gatgebalc.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gonnbtkgi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvmnvlxs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbxlyplf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gucrqfirz.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkedsymqv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbslgbqrk.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gynbfmndm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gzeugdotb.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gxtvxydyo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/guzhbjzqe.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwkivkxpc.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gunpopone.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhkvicso.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmmhnlwq.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/ggxbjmvcz.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdvaingco.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gntjzhmrl.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfdanlpj.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpxlsxlx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjosuqigj.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gffcmvkow.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/goqrregon.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/glwgqoeqv.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnnoyxmb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfyzhfzs.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/grlamfexc.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbjdhkxj.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbpegpck.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gqsctsgff.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gtclgmcvl.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glomwcphz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyswkwwv.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmwsmhdp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grusueuqr.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjlbnlxy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfrjjoed.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gywypcxof.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkdosygu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmohckqby.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gnrxdskju.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/ggugvkthc.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggvuuaxym.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gzcgjucrw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gaikkupdp.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcfxkrgsf.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/giynpblol.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevcipoew.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/guuhtewgi.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsfwidko.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/ggqzcycfh.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gviuiziwm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugfwakts.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/ganfkxndd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/glptyysdc.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiwxmeoj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gmmpyrqgy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtklbkgid.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gxmfqiarh.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gzyitemoj.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gvulwbnfk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrgksmxm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gozeeeafb.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gznmeyvrs.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gdbsigrme.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbesfzau.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmawbfuck.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrjqovo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gratimqcu.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gvggmmqph.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkeqnapk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdhqdrdg.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnvkyeqy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmzpfaax.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkxzdpvo.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gjqhqxvob.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkesyiyav.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grffzfpiz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gllustlph.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gjixnkhba.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gilcrdida.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gazhhmumf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqxiktjer.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/guhtpxdpv.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gaoksfeln.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gepxpaptd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/goaynwjrd.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeicgbmn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgbtwisx.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdxuznac.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/ghksqiium.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuecwljc.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gdoljryen.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbluqczc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkczbmvuc.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhqricsk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gaokxbqjm.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gvtmwxsux.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruojnlxp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyqqqdcgm.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeuioaqn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnrntmlu.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzirzdei.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpljmuyxl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gocgryjin.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gpwzlzuhg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjsxkbma.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/goylvgano.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gjgqpysia.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdxolsix.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gcapgekzg.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxblncqg.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzdpiebji.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goilpteqq.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gvfrlhtfr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxtlczpm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycgdyblx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/grtfdrpoq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnokjqqih.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpausbvh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gxxpvpyxe.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/ggmvcdhca.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvvmlthg.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuyvtfqs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxpvqdoc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjlsgmtg.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gpqwmevep.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmyudtsp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiheusbl.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gubsntslb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrxgffqz.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/geqtqluzk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxxneywd.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gfsjokfcy.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbbmvjlw.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/ghxogezzc.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gqsvaajzk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkinxkcli.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuelrkbm.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gojndxpha.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxovuush.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnyjkfrt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxgimetu.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnlzxxxd.sHtML


<!-- 参考信息 -->