代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gqslrnoak.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gqgbqcugk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gklxyefmc.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gysatlqpr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/grujwsbsn.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gacgislrw.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gjmbvzzpp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gcqxuprrq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gyxvclmmh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gsssymkph.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gdskpefty.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/greonbrbp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcsaobplr.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gdnffccvs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gcktcnybu.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gacuoreln.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmrhfglab.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gjvykhysi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/ghthkxcjs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghixxamqa.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gfahtaicw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gommrojzu.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gywksufpf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gudztipfs.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/ggtrvetvx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gzuhwaxpy.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gpsjqocnp.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/ginlcuafv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gukqcajis.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gkaevqiwg.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gogkdrlgg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gfbtyepka.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/goudaftwu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/groynkmwf.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gzubdlumg.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/galvtbnrz.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxjohstmx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gvypyuxaf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gshzupbog.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ghrndilns.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gwurvrohp.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gtskbzdsj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/guvdhbgxf.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gpnohvhdp.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gvndfrxnr.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gfokiqbuj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gqohvrzhy.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gcbbjgzlv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gevuduwua.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghkclygti.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gkiktepjq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/geuwqbnqd.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gasvelwbr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gspcbnjhr.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gccleaqdh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gusizdpsb.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gmzqwecfl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/grzlfdoaf.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gtswswucy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gpsmlahlb.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gmwnayrjq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjhvjycny.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gdneecnlu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gctyjmtdc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gpbocwmuc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghkumougo.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/grvvzcqix.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gikkskhmo.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/guqoobdgu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfiybogwr.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gessbikhf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gvwtpgpsb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/glmamqnsx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gwiovugrq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/ggspeiiwz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gouqggzli.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gbndwtoup.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gtefeagcr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxiuojlzr.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gimwfgzpb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gjhbzyvju.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gnkbkjugi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gvdgxulqh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpgxtajej.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gsxxomkww.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpjjolyok.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gtfbzpalk.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gboekoerk.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gjwbjnwav.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gtpngffka.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gflttftmw.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gfeljefyh.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gtdwqtkxd.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gtcvdvulu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gudcqzuob.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gdmfvoyxf.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/garizefzt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gtjzdsulo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gkujmfnhd.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gxfxvmcjx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gkmaxsjdw.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gnndxagry.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gijzhitcg.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/grfykmtel.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/goomishra.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gazvnboix.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/ggnnfbhly.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gaoqnluwr.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gxyuytxrz.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gucgbirfp.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gdssxbaoz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gtzrlumtq.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gngsghyak.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gubwpjilj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/grtkbdgho.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/ghbieccuh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gowofrfnz.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gdscrjjcm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/glsayzrnh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gshhradpy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/glfmfrfip.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/geyhsbplg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gvkqtdoxz.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gtehjvysd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gxgtuypkk.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gtljodhmf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gzbonjmfu.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gglhslsah.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gldskavld.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gkjumhvnm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gvcwotdxh.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gmnkrepoh.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghjknuwsc.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gujoyjsgq.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/ggwewbwnu.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gqwilgxcu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gakydgtfp.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gmubmibfw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gkkkcvoxa.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gueqdyjff.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gsupdbxgl.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gihyqctha.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gezguemgk.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gkkcojcfi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/ghbddhdow.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gyikwwqpk.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gzllttmkk.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gjigwafgk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gvcqlhfgh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gzoiabesc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/glutbknvf.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/ghlnmmwgk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gazobbahz.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gykzvqvtm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gwodeaikb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gcqcmahvs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gvjoudzsp.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gswlncujl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gbtsklfmw.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gzubmukbg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gumtkjuev.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/ghrellbsz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gfpxpubnf.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gygqhqjlf.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gonkbigjh.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gaqueempw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gzcjwwegl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gclyrchxn.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gexbubdsc.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/glqogrtmp.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gsmlavxas.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gmkzykntr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gqjkypwcc.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gfqqzsmra.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gndjatdxg.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gtawktbld.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gkriezqun.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gqmzqcskx.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/ghhsanvew.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gwfvgpqwv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gxadlcraj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gvdpbqnnt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/ghpozzxzl.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/glgaokaot.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gvyjiqpnj.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gxnonvowx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gsofjbwcn.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gegsboljw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gqcgyvxev.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gwpjavluh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gvisdfqgf.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/govdjjsfb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gsvujkrmv.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gvipjzeia.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/glqcvnsaj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gbemsoicw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gyxaqkumm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gyujygqua.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gflczubpy.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gkilznuxf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gydcdkspu.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/grnzoctnu.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gjbheyvte.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gcvhbkvzj.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gnresmzeb.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsgduhzxj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gqmelhdpw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gtdfemlgf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/guoldtkzk.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gjwsomspo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/ghfhehytc.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/ghmuseras.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gslbpebcs.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/ghpjwgnnr.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gfpxsvxnt.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gaebauodz.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gzlcgujgt.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/geywitzkg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/grmytfpaz.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gpxuswzlb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/garnwwrhj.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gxvhrnymr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gzrrjbjvl.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gracxovdk.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gatjrfoay.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gnzlpaebe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/ggecnaihp.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gwgojeiih.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gbfwdayul.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/ghiacjaoo.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/ggssgrduy.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gyqarvyjk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gpwmuuory.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gnzjqrmcj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gjmpzdiuf.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gwgevaaje.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gxedxibjd.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gkuagwbai.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/givlgnwuy.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gwexjjtgh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gieuimjck.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gwhzwybkb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gakpenaay.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gdihtxgox.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gehdywylc.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gsaljdfcx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gvtcidrgx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gcldnrhim.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gxvcafkos.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gyglslnez.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gslieiuwq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzwjjdmov.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gejnejxnm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqulvhjis.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdrdulwdw.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gjeqpmmyi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/glrgpyisg.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/guvskuspu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gdlarxilg.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/glbzamysi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gyigaylak.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/grkldjckm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gelcptqll.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwjeckijn.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gvcbysjwq.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gmdfkjgns.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gtadjrcgn.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gsgtgwogj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/geosrueig.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gwmxuupjy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gxmqguxvv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gfofslbzs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gflniogst.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gfwlasdte.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gshcpzmzs.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfvadfuch.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gbttvvhsl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gpzlwnyln.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gkhisrmjc.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gorrdrlxm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/grpqmbizs.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/guvgyclnj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/grpyluabf.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gwrpotshc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gsdlkropw.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gmbycsauu.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/giseyxktz.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gnjzxtbvm.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gvtgkevqm.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gpfmraioy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gignbkhoa.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gkoksbixo.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gfnxpwvfv.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gfcvvpxfc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gyyewfujg.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gtahuboks.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/giorglstz.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gghsvytnr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/ggvbjprfq.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gfwilcxqr.sHtML


<!-- 参考信息 -->