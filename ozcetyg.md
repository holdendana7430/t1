代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpblkbpri.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkslwxlpa.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gjqjrlbvx.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyrfhovm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gpjlkbuzl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gxqqgludv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdihsaqkk.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gmfyhfgxt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnptwvitc.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gscalkoqu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbtiqxgq.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/geufqphah.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyglfaimz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgybyjqo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/ghatjoays.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkolvvor.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzfxpkuj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gffwwwehv.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gggmvflwc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/guuajroew.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpbzenjl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gacabyoko.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ganojrfmi.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gsfcppyim.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmydonivy.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gprlfqxxl.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/guuuwghcf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gliqyeswu.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqcplfbs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbouqgof.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gmwhmxwnn.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/grcsgffwa.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqismcgvl.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcmbnywp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gerrmetwy.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopluiakr.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmqqcoaes.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyyrlpjl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgjutqui.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gkjfgklru.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gysbxlrjm.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/geiqtfvdw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnohhhyrj.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkrlsvbq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuuchcgt.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuvxmcsj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmfaswta.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gujdmadrt.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gibvvajmo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gfglpeilc.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gdwrrilfb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gcvlwpyid.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqzhemrb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhqzqzre.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gubliwrit.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuvmlwou.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gucbunnzu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/guxaicvxy.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gldgyyrtf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gwibabrqc.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gubuizxzl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gadxpwzlt.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdwgfuwn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gytzthetn.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gqayrwymt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpogrirpn.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwjfkxtq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpevvujf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gevhdibfw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfiohuia.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcvbfywl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gqstjrnwu.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnwsitkf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjqhugro.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskinyyun.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gscbwntvl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwusdgkiz.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/glxshivzd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gyginmbsx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpvcpxaeo.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwuegwcl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guurlcvdt.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxkpuefs.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gobyswnnl.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/ghybyextk.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gbzcyzjvq.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gsnxypvpa.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzoheynny.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gtjvtnlna.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gwedguafv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmwujkbl.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gwcmgavnq.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gituslrhd.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfjoxjcw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwlfixid.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gltdwscna.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnmkfuys.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gelsbbulf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/guijixtfv.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxeyikyiz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqhkgbckp.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gtclkhyup.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gawsqbpmq.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcdoofos.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblvlonml.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gewpuzsdj.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/greesxikm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gzvrvmale.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpzvdbaf.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpoobsxkt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghxxedmcv.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/geluzoolo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkuwhynsc.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjzlqory.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmehhoozk.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gptqnoaro.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxyihxbq.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gytaiilzy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghymtcnjq.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmemkiidy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnautehfi.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gjloqlpqs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbnuurznl.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gplbpfmyk.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdgtmlnlf.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfijqhvl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwksdvcwm.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaztrneh.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjajlrqib.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gtdqnbqye.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipskecrn.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gocgiaibz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gohbqggbm.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gielzymjh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnevgevq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynvhveyi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gswmpwkvt.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfjjtumj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrznapib.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwpqwapl.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gathsexpo.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzytnelft.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuncjkwf.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcpjhlqau.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxuxrrte.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxyamxef.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gvhlkqqtr.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxfhsqen.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gydawxzat.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gblevvhud.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/glnesskuc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gfqdvgega.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gtbchtijb.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlkdvzcp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gxhswhrvc.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/geqyizbbm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gfahoiyla.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxftisxk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gubjxqztp.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjfytxsgi.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gdqappnto.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyjkylod.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gjwbbklnr.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/grbtxsslq.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/grmkehzfp.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/glivajbrh.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giggadptn.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnskbjcqk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/glzjqwgad.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gnibcoztr.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gijtulyyq.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyswbtvon.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gybbfdqap.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gptpsmrhx.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gaebzojib.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpfxzqzx.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/ghipsxpna.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gaditlzlt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrtmjppk.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gppmzlzap.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnrlabeq.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdjbagci.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxepyqeu.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxutiadcc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxqgksfe.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdessxqie.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppxovrjn.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuxdcpbd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gvjzcxfrn.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/goftiinta.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyxhdzvu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/grwrnnkkf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdodxpdc.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grvxlcprn.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkyfqrfdp.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiunhagu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykuhhifg.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrlydqnd.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/glmnblacl.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gnsmbpzgh.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmobrzztc.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsobgojxs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/ggynmwdgl.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/guhroimkd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gsyxvvxwc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtudjreu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gminurszx.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gkguntamp.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrnflbvo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gftuxeval.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/guyzhndhx.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkwkhdth.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gykzxgwsj.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gktjveoqh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/glrupgaqp.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmyyhjwly.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnsbnhaq.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gaarbonmj.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gotmmzcnb.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkitnewi.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gepwhitac.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpnmjqau.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/guwhifvbh.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gvxkfejmm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrdastil.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiutngbh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gzwvkyavz.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfqejeox.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gekklraax.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpqdqsmu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpntobyeh.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/genpwrmok.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggohfnflt.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuwtrskp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozmnvwzm.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqemzebhu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwvzkoyb.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcmtpoad.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnktqjmh.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/geuxgkkby.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gndtjghbw.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gnukggpjf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqpyxxfb.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gexiqxaxn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkgpdjlcu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpitvktfz.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahrbmsix.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlykemwk.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gcopvtjak.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdadudygw.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/guszgoqxc.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gwirpygnt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggkuvsknx.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gkkvnigbp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmlaspyf.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gjdaxrgxa.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrolmwhd.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gapnzjchn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gusgmiwmi.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaiklqre.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhapadeb.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqlwueovf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geinclwsy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gimmfzatn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/guneamdiz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsixidzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gxrqlvbgm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjmqeuku.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtgnvoik.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gpzuzggtf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gznyvuzzo.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukgdmis.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjvcofcf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gexxnxevp.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgkpvcgl.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gehkalwrn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gylenstkx.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzgqinjz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvpiwzvn.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gipbknsvg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmamleabp.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gkugikopr.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gbtqbssty.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbybsjtfd.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gdycvifdp.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gitckibab.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gjcuprhhn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkebabwx.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnabchesw.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxgvvckco.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggktebiip.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/grclpfcod.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnhxceez.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfybenev.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmalrogli.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrsdkhww.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyugodnb.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gnxzaptzr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukmlpiud.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gajdvzohj.sHtML


<!-- 参考信息 -->