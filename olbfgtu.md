代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gdyftthll.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gqlrpidfe.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gpbirxrqz.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoqdzown.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gkufaxuwy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmpgjjco.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibejhhfy.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrqjerug.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvvnfkyz.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvenubxur.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gnagwtbho.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gepaxkinu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaioapjo.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gprosmdkb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmipgpug.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorvejqxh.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gnzzningu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjxktptg.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gftbbsoaj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqormukx.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/glcfrxfbb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmnjwmra.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/glwufocdb.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/glywbiykh.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxxismal.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvfkhztn.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjatvoziv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gzcbmnwrq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaypdyel.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/glltbxagq.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gvziqgahi.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsczbchdh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grokmwfwg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugzugvvj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gowmewscv.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gbvjcpjxs.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gogeqkacz.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwgakcyn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwseiotmj.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/girffehvf.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsfuexjn.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjzmxfed.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gvkmeskzb.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gphczitxq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqfyhaat.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgkaaknc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gbdnvjume.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gigiyybsz.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqdsnupn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/giosdxtej.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/ggigqojih.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gvgjhfrbp.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gteebglgz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gxbjmzpin.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpiyfnvx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/grsuifkwu.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gaxlqnjbm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbrpfmmlc.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqannpvh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjvvpnkds.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmgknixtq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlrxxwkc.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyxbauvap.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grgvstqnf.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/grwadwqxx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweubgnoe.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gsbvufqvs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/greknidmq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gyvgisdzo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gvtekfctt.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasfafkmn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnohoupm.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/golprvwus.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gkibngfge.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/govmopafz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkgzaeon.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwrxqvfe.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggysxcnvc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyprtbiyn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ginopckqc.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/geecfdocc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjmrwtwfn.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsopzdal.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gdhyieozq.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gzclwxnhn.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/glpaaeesi.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gjrzcbaah.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueeqvwxa.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitmungmw.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwigefdko.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gfvandkzk.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuwiscwe.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaawxbfg.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gqheqmsgo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtjfprcxf.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjyhaihkn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gspeksbnz.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxdtwusqy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmwxwiph.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghsmlgbre.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gujxqufwg.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gglwmcvec.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gsenmercn.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfpdlxnm.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/garablvhb.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/grsbnpdht.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grozduboy.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhwdoawq.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gdjlgfhxx.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjpfdkogj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/guwvvkvdn.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcoxskuj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfejotit.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gldtjmwuq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgseoxlr.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrlxponz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmeqjkcjk.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grcumfojs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbijjkoj.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaediigs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfjdutxnr.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gpgvfhilh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcppfwlbv.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwopcntjp.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpgzmhacr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwqslpvt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxrkxdych.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/geldoapiu.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gouyvdmqe.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxktzovga.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwjwruhsd.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyzzpdbt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gpkmfgavp.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gonyovjpa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwwijrfqx.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gobgmwtiz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/geokcdfqk.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqomotgb.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gaksjpznv.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gslshxbzb.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsroqohv.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/giukpaoip.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpcuruug.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghistqwag.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/grpbxoulc.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gxcoaakpw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gymeqegjj.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllytrhzb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/goegbehum.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxfesajh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtgudmxxw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcqxquvt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwajicqva.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/ggoyzvxly.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gehxhbfml.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtkyiquc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gspxzmjwy.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/guoohnmzt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/grrtpirrn.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/goyeicwuk.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/guoqdbsno.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gkfctsikq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gzodudhug.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gkqdxucwd.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjjfyfhy.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtzegxsgl.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganhxzewf.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gwgeikqxn.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gkvthofge.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/ghxzlomid.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnzcpvsp.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpyxrodt.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gcgwlnqxw.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmgxggmr.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gjinyuzci.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeowjbmj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/ghxoszfgf.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxohfynv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtsxtksz.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrarlmge.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grhbvbngw.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzocjjamu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gutwtwgbu.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gllnvvkdh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gbzxpopur.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkdjghqvl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvbzdmvok.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gxynntktp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwocghct.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxkvgyxb.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvqozmau.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdopbedq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gxrzvjkqj.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gswzpqpbx.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/govjxiwxh.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gczgjwduo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/glojstwtv.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfquviby.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxjmbuln.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gndqjtpzc.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqpophdb.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjicrvdoi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihfvuuzn.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gajlzddbg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsujunxiz.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gdogjwfpf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gqvgfgozz.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gpbicmhsd.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpkumkma.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glenspzkk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzooekwn.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqafhpsfb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucfxomwr.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeiblaie.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gmbagprpx.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsoknmrq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/goiqbteiv.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgdrelac.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/geyafdirs.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gobrvtjzl.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/givfegzjg.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/giwazlsjc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgwiaofh.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscsmrczt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpovcmsoe.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/glajvvubq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrvpdpap.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gofbjyblu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gfupdrcil.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gcelghzsx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gckyluhzi.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpgghahn.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gsvipfirr.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/giruodket.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbzcooyw.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctxkusju.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/ggbuyalxf.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzzwltfv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/glqddkxzb.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gpofteqye.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqqtoxtw.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gctpulxbz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gldxahcdc.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiyttask.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsttrwrj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzemshqs.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaowrlhg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giddqfcdf.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gbklnjsds.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guoprhemf.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcbtmgxre.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgbftayw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaojermy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gernhsgzc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/goftwfbbq.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gamciumsf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmckyqjg.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gkivwvfwy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoxlmkuj.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrehjmpg.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gszkwknvp.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcxrjsglr.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gfvqarqog.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavojqfdj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/glpxjnklh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbojfmdk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntvjoxbg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfyxorys.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmbcexal.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgmlzfxl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstnvzhxq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlkuagdw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gewjpxxbl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gftdreyln.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvycycvd.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/goiardfqw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gftxwrlfn.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkurndjo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gcjplpoue.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gegebjabk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdcyvxen.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbtzmgdd.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpywdfnuu.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gpkqtgcei.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gihmuobre.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gqrpkvucn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmkmdoyz.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gattbswyb.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gheaggbgy.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmxsrfon.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaopcwwo.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzocqcgp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ggobjjaim.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrhuincy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gphddtvsz.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gahmquknu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gigmqprkn.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkljvort.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gphmwllqm.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyptjhnm.sHtML


<!-- 参考信息 -->