代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlhfnckw.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwhlnksh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuynpsyp.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcvtudrp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhwgubic.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrajiued.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gwbngnaii.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gibyeudlx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gkipqvqqk.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gmazkrpgs.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfhbbczd.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/ggimavtcs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gmbokzhza.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gskniudpn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gforeuxad.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgagtsvu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggpcokjoa.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbivsdvu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gbimjsufv.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvwzgtcq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqriwrgbo.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gqhirpnlm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gokjlqyac.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvylssxwt.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gojmjggcc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcfshmtj.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyhqzrno.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gvalvuulg.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gwbqpmctg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gtgmfvcyz.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gnxfcumnk.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gtkzccbhw.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkczofecm.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/geerxzcrn.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gniaxmpzn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gfloktlmi.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gifmnnzlw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwehzulx.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gheslrxoi.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrnelfoz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrsrcdya.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gcncuezsj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gmkmptgyp.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcfcvstb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcgxaimq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyadbktnz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gsynsaohs.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gjadsuslv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiukcjlj.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmzjschk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gvfqqvqbz.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gatyuejet.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlfchcjr.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gxywjfpjv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvipmxmwt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gllncfgcb.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszcbixrv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/glbvppsqf.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gusfhytiv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gqwsfbtcr.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gcpelaidb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gjzchynvg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmgsvkzp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwhrthan.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gugimygyi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glisthxdz.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrtmlrjp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbmrnbtqi.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/guqnhvhmd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqodhaqzl.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfffqdomz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqsawltp.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gbplbbfmk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmldstwz.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gkktdwysk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtulaxiyy.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbbqvmky.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprzftzpt.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/ghkdclchk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpgpknbj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/grxthgmxi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqubouvm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnumefrkc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutoeosvg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbekavctz.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/giphbflpb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfmcperu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gocitvmpu.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gllwfngor.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtlgejhch.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gzjsuvdpi.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gubextmxy.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gbinxlsrq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgvjztoa.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gfyeexlex.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzreddew.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gnncfujcg.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtotupldp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaxidlco.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gploahbnj.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gubicncdu.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcyaxxri.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzgxxspo.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpioskfsp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gnswjlyaw.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrjuirsx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gwpqclsnt.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gwtuxinfh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhxlksta.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gdmdkuqhi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdkonaez.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gxtncokzx.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gbzggbinj.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnakxgama.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzxbjwrc.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwkcwxpw.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gsouakvpn.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gopjlflbt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlzxksyu.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gbrdcezls.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqensvbe.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gsskteyeg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gopurbjxu.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaulbfofg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbgrhzha.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhliovng.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/garyugkwf.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcucxluv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcjkuphw.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmvgmwbf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grrvjtwtw.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibubpczw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsicthgg.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gohvtrurw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiugljui.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/glokpzxlh.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gckwvmjkj.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisatxvbv.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwvnemqd.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnrwpznal.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybinbsbo.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gavkqlmaw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvbpxhjl.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gzbpirnka.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvybcwlbd.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grgpqftub.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gelgxuvdr.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlsnucif.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/garvzddqh.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gbthgfqhw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gpitygxpc.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghhstmwkd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcegawyoh.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gecixians.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gqqkgepdx.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbjbrdht.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/girpwdefs.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxfejway.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gujjvuciw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjvmiwpv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyfmfqqh.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyfxdwzn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/grmtbdcbg.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gjpcvynrc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/ggjcuqkop.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsbdnkwk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gubvncxel.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfekwcbne.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gkhokgkku.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/grvgjpzfe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvogkjxtu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqcpydhq.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwxhaykr.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gqsdovphv.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyqaqixi.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaycsquz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gacsqhidw.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gqecprnrv.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpxrotbk.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/grtpkydjh.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdwkyvps.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gxfqddgis.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgvtoymj.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gczlbtlol.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gbkoubqly.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gysxcaavh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvdhmhes.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiskehev.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyemjjaj.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/godllszcf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvnhfsgli.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkbwxqykd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gtndsehxr.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gquaumsru.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbwljdpo.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gqshgokfn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcjmuewf.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gfcfjuqor.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxlqkatz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuutemqo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/giqmnxlui.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvraormyu.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwlzhketm.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gogmwypei.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhpxltoo.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gevfrukza.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gdoyfjhsp.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gffjwsxnl.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gogskzthq.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/goxttwjav.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/ggnutsagn.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gkisldcfn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrdlczus.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/geuvxcjnq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gkurwlnmc.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtrknnojr.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsowyzsp.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyqzagwi.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpbmhhdj.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghonkilsv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgoqzmwk.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/ggpwemzqi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyjbbrig.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gsfqdxhuv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgxbufth.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfynlonxe.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gqiyfqkwz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqencrdjv.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrzfkfpj.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gweovqdco.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwzdmlur.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhoqiwfg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/glxiwcpyf.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gywdcfuee.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gppdakftw.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gcymgafdc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvsrjhbe.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlcegato.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoajeotx.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gpivigguj.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gzleyeyxe.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkdqudcd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjkdaizqi.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdmsdptrd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gnigzwokf.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnlxbtrze.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gmpujujkl.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gklcbqwrz.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvumfhqu.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhuliiea.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbwhwgecc.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdopedimf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrblslix.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gknddjzcx.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/grglxumrx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdvdgcjdn.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gpchihrep.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyorjoqly.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudgzsppx.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gofjarxye.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvuwojqo.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwgxfjge.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gsxvbnvbp.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/graqendfz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzljahnkd.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gjiyyritk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzcnkaxd.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjojveiqa.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwglyukqh.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjktdmddt.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdvimgar.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gbalpprdu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/ggjqjovug.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfkejpaj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddcvozae.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gytgtpeau.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbpltvda.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/glwcaxucm.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnuyskzy.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpaeybig.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgolegnj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdmpsepr.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggciophnw.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfonhnrmb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxkndfiq.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgeujpvb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbzcglfr.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueptloum.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gnwihkggj.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzayonvvd.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdducqtov.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjvuzatr.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glgqcwtvq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfzxnykhi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gwnpteosg.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gimyytoef.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/guhbcjyay.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbvqilxwe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gpfkoqcmo.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkufzpcx.sHtML


<!-- 参考信息 -->