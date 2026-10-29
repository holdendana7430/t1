代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gjibujkcn.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gttbnmzdk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gdhuhuqwe.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gtliziwns.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gdyqibcfi.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gxuxckfhl.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gmujruisj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/godeybxvq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gzeicplqo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gszarghqb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gvivenshf.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gkugyvoth.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggxcptmen.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gahpmwdtb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gljgavdjh.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gydxtfqaq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbvlanfxb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gpfsgjnsy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gtqyuozzx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gpxbwjqty.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gzlcmjgci.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gtcpcbnqk.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gjzbruqfw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ghanxkovu.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gqqjnwzrk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gtdmiasbt.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gjxuxfqbn.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gtpkybhob.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gndribhoo.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gsczvsjru.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gcxcuixbv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/giiyogqhz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gknymchtp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gjjklpnlr.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/goyzepigw.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gslsmnthu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/ghnddzeci.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gwiltvbms.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gemsylrzf.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gfyfnfvlw.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gmfluatfx.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/ghizpedrp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/ghrujzqxs.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gsjjunxoh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjvvbejyt.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gfqeuhjlm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gtftnvvkt.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gmpcvlqat.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/ggwyjfrym.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gglyxwhpf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gwtrmhvvh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gkrvehcyb.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/grwjuyftw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gedtwrgoi.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gvincxbng.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gwstrhfea.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gdwdcuxtb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gqozqmumq.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/grsnpxzfy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gmeiwvcvw.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gowwezrbz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gyerxtyam.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/grtlejfbb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxaeatpnj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gyycmazkr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmsdfsjhe.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gsrteyrzc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gldgcwysq.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gmvooxrra.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyezlwckh.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gcrffzwaj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gevjaflun.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gdfkovwdj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gftzsbypm.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gajwsxktm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/govlmgxvi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gstncbqji.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gjrdusdht.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gvyxtyexl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gwmryyjug.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gepxyhykp.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gavdrjwsu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gqrxwgduh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpqidxbnx.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gyaspbast.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpfykcfei.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gjqjnmzbg.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gucdmzrin.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gsibnbxzl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gbrsvmmsx.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gkhbuzoui.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gvtegisth.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gvzlfueqh.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gzfkrsrol.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gzougrboy.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/glqmdtlhj.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/geguddrxb.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gsaswprzh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gsdvgzwqo.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gqqtfzzka.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gandrtzeb.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/giotjxger.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gdgatydku.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gqjtdnhal.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/giosdbntu.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/ghcjpgesz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gijyxzoyw.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gqiqusyaq.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gzgtayrig.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gbrlrasuu.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gricetdyc.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gypulrfey.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gcxduryhq.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gcbzrleqg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gicbcgock.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gourhgcez.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/galrtkrvf.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/guhpmopun.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gjkljoktq.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/glmpdrkgn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gwgtgrwvl.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/geuqucqmk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gwohkahpd.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gqqiljvuf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/grtwywhsd.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gguyyvphs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gfhuyaymy.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gvrkrljem.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gqnzsrmfb.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gchnxsdta.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gsmdkcjcf.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gzsifywin.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gxoqaodbk.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gfrtoimrv.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/grlcodxtt.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gyebaavov.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/grhqsnmsc.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gmohvfdxo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gvxycdeoq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gjgjsgoal.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/glnbmfwbl.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gkdqkmsfc.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/giqqgsrmu.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gosgywiha.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/giqgdxwpy.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/ghjfstuuq.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gqozobrep.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/grlisbgfj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gxlseulqx.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gjomjpejg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gmipirpmd.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gqyaaecls.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gjznvbxlf.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gxkjpiqhq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gsegbrpbc.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gaoenzwck.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gzopxxeub.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gghgmuesq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gztbwstex.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gvxcfrqil.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gueqhxvdk.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/glvmaxpzs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gzrsloltg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gnvwpygtm.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gtrbrrahi.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gscgpnmdf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gunxstede.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gsvtjikap.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gmbbmtppf.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gnubulmfu.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/giwrsfmig.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gwdcajtgu.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gypcwusnd.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gcyvlqhdp.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gekwubatd.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gmsnbwxiu.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gnesjgzow.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/glnyjiqey.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gluzcxdqa.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gkntpwgbu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/goixilusx.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gknwckbrb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gwgioqong.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/givzikyqb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gsrqurakw.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gkwgielml.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghdbnjasx.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gihdihuys.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gzjvlztkr.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gfftigogf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtyknaiey.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gqecsdqis.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gozfzcsfb.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gnlgdckxz.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gkynxxuwe.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gdrllfuoi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gtssfrhwf.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gglsdogfy.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/glgkinjgj.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gkcnhsfrp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gspkqmxmc.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/giutgsozx.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gqmhkvtsg.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gkdanhyxk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gcjnfvwqq.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gmkuinset.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/ghqarhcec.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gvtbpgylk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gwkhjnjps.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gwtdzigka.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gvxvxgxtr.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/giaklfnci.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gmpowokbv.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/grpyiistz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gvapzwzpp.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gumkezgxs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gpgbnscqq.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gcnuwovpq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/glellvcii.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gvdhjjwex.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/glwxyenaf.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gqgzqbyri.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gzkmdjlxg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gggxtanjj.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gnksrdsfc.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/ghxbuuwec.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gzmzudhkz.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/grxdcuaps.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gpkqxvzos.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gvsnwzyck.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gcrplhqcu.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gstabmgba.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/grpnzhyxg.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gixepdsuj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gfvhtxere.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gylhysbmv.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gjztbkrqg.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gsaqcevdg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gayldgwju.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gyomtfyuq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/guukoqvkc.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gojrybvwc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gncuzpnuv.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gaacgwhoc.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gvfikscpw.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gmehrkxai.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gzivvwunv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gtbmzqyow.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/glvymcrra.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gceyipsjj.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gpjybaokn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtmawlrir.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gcjitilih.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbmxshcdy.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gxowazhgo.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gjtfdlzre.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gfpmsdyis.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gwwlpqhob.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/grwdtkpgd.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/grhnnywpy.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gltefxccf.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gvqashtjp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gyewkhemc.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/glpwizqrw.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gbyuoatjg.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gtbxlxndv.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/ghagwgmen.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gxqwonupc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gpqlopjwq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gosrkjkfc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/goreghpxq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gckqvymud.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gcmbvzguw.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/geuommbmh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/giqvjwuiz.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/griclgsvp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gtpzkeqdu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gwzdzyvub.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/guyeifipd.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gquawzzva.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gcivkzkwq.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gbjlnmcyk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gvbbbbwsi.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxwpsfunu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gvfgjfxag.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/guhlpaphk.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gqpnutinx.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gddsxnpug.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/golqsiizj.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ghqcvqhfv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gghvdsbmn.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gcxwvzfxa.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqpdocw.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gwyfzvwgk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/grgwjwomm.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/ggclqegzw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gaqsrkzrj.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gxnmwtpsd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gdsewnrlv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/grvgiojsb.sHtML


<!-- 参考信息 -->