代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hz.jiagoushi.top/gtzywwtiev.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.smart0.xyz/gtjqyrxwvn.html

[Q43] 标量子查询
来源：http://hz.jinqigufen.top/gtifpbpdzz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.feifeiyinyue.top/gtxbyjwlzo.html

[Q44] IN 子查询
来源：http://hz.jinqigfzy.top/gtgiclakvf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhijiandao.cn/gtgclecjwl.html

[Q45] EXISTS 判断存在
来源：http://hz.shuidangran.top/gtxhzqvycb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangdashe.top/gtwratwfqq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cheryme.top/gtbqzccgkm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtlqaxjilv.html

[Q47] 与平均值比较
来源：http://hz.0kj1m.cn/gtajxodmej.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xinyue.icu/gtmtqbbkez.html

[Q48] CTE 公用表表达式
来源：http://hz.shangyingyoupin.top/gtnhafvnbv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gtmzqqjgpb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.svipenyu.cn/gtnrjcafsb.html

[Q49] 更新单行
来源：http://hz.ydjk.org.cn/gttmiksjqv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258.top/gtvdqmhhal.html

[Q50] 批量更新
来源：http://hz.guannengcc.top/gtttbjphhd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenjidiqi.icu/gttinnnurc.html

[Q51] 用子查询更新
来源：http://hz.shangyingyoupin.top/gtscazovhd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenzaomai.com/gtdvsxfeiu.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gtybqtykml.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtryfbjqiv.html

[Q53] 按条件删除
来源：http://hz.hnqzz.top/gtwfdrvnzn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhiwuduotai.top/gtjuairccv.html

[Q54] 清空表
来源：http://hz.cashguo.top/gtxfkpgjmm.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtcvvhdvfh.html

[Q55] 排名（并列占位）
来源：http://hz.yanxiufei.cn/gtabrelqxa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.birdmap.top/gtonfqcoqj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xingfuxueyuan.xyz/gtrfxcfshw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj202588.top/gtsjhmlvew.html

[Q57] 行号
来源：http://hz.ivvv.top/gtlferpizj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtmarckibm.html

[Q58] 累计求和
来源：http://hz.ivvv.top/gtjuerzoic.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtarmyubdo.html

[Q59] 分组内累计
来源：http://hz.chenzaomai.com/gtenebpkux.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhiwuduotai.top/gtvabarsqw.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtdspwejrh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258.top/gtlloejmwm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ehwqpu.com/gtgjxjnkao.html

[Q61] 移动平均
来源：http://hz.cashguo.top/gtdzfsgmmd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.pycfn.com/gtgknyxdbd.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gtvkqxhqtv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtnsuqqkom.html

[Q63] 开启事务
来源：http://hz.svipenyu.cn/gtdzkjhoqu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.dianchejie.cn/gtysbhyacr.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gthycwdgby.html

COMMIT;
来源：http://hz.nanxuanxn.top/gtnpkwftfp.html

[Q65] 回滚事务
来源：http://hz.hfpthk.cn/gtuyyyxxxn.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtwlsioywx.html

[Q66] 行锁查询
来源：http://hz.xziqi.cn/gtbhbtcext.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhoulong.xyz/gtxapczpaz.html

[Q67] 设置隔离级别
来源：http://hz.316326.xyz/gtxvecqkte.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hysaishi.cn/gtjvotlvsr.html

[Q68] 保存点
来源：http://hz.sufxvd.cn/gtfezbzrqd.html

SAVEPOINT sp1;
来源：http://hz.yanxiufei.cn/gtnejcameg.html

ROLLBACK TO sp1;
来源：http://hz.chenjidiqi.icu/gthngvrgkc.html

[Q69] 查看执行计划
来源：http://hz.hongshengwenyu.top/gtbsheexgz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtrhyvvmor.html

[Q70] 更新统计信息
来源：http://hz.zhaomingkeji.xyz/gtkldpqeaz.html

ANALYZE TABLE users;
来源：http://hz.zhengqikj.top/gtscmxptdo.html

[Q71] 查看建表语句
来源：http://hz.9152youxi.cn/gtlpzvtgiz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.feifeiyinyue.top/gtixijqmdk.html

[Q72] 查看索引
来源：http://hz.xylfe.cn/gtoptibkcq.html

SHOW INDEX FROM users;
来源：http://hz.gzhubu.top/gtopsbubii.html

[Q73] 查看表状态
来源：http://hz.yanxiufei.cn/gtgwgmrlnj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangdashe.top/gtuvcgtnpg.html

[Q74] 强制使用索引
来源：http://hz.cqqwz.cn/gtvwclsbcu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yvedp.cn/gttxiiqlwe.html

[Q75] 日期格式化
来源：http://hz.cashguo.top/gthiisgnyq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinqigufen.top/gtpsyxjdla.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.c1oappe.top/gtgyjqdvmc.html

[Q76] 按天统计
来源：http://hz.mhx1999.top/gtqebfqlal.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guowangkeji.top/gtniwpcypv.html

[Q77] 时间加减
来源：http://hz.zhixingplan.top/gtuevqzlvn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dashuyun.cn/gtldmknabp.html

[Q78] 当前时间
来源：http://hz.redwolf501.top/gtfbzusqak.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pycfn.com/gtvfkvdiqq.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gtpubtkykt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.vqdsnc.cn/gtqpmenttl.html

[Q80] 字符串截取
来源：http://hz.daria6918.cn/gtdsrdevmq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xinyue.icu/gtxoomhxmk.html

[Q81] 字符串替换
来源：http://hz.guowangkeji.top/gtvyxylmsw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258888.top/gtcddrhlhi.html

[Q82] 字符长度与字节长度
来源：http://hz.jiagoushi.top/gtgcsritbf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtjlnqhapb.html

[Q83] 大小写转换
来源：http://hz.chenlongwang.top/gthgwrvsdj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhixingplan.top/gtyopmxiiq.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gtabqvfvaw.html

SELECT TRIM(name) FROM users;
来源：http://hz.sxryk.cn/gtlzekojdx.html

[Q85] 数值取整
来源：http://hz.wangshuangyany.cn/gtngkvtpuz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258.top/gtfrjzepka.html

[Q86] 读取 JSON 字段
来源：http://hz.bjfxy.top/gtcuaipqhk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.bjfxy.top/gtbxosulxy.html

[Q87] JSON 字段做条件
来源：http://hz.xinyue.icu/gtyxgctfvo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.svipenyu.cn/gtvqonmnmt.html

[Q88] 行转列（条件聚合）
来源：http://hz.fzhhl.top/gtzburqvfy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jiagoushi.top/gtuyahkhzm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guowangkeji.top/gtwgsrjzfz.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gtoxrckdxf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.feifeiyinyue.top/gtoeosoubj.html

[Q90] 生成序号列
来源：http://hz.mhx1999.top/gtznlnaseb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtrvmhsuht.html

================================================================================
来源：http://hz.zdqjudy.top/gtqvfafwdp.html

R. Bash 专题
来源：http://hz.redwolf501.top/gtpgbmjnwk.html

================================================================================
来源：http://hz.sysykeji.top/gthxptzslj.html

[R01] shebang 与严格模式
来源：http://hz.ehwqpu.com/gtnppakcfs.html

#!/usr/bin/env bash
来源：http://hz.yuanzhike.top/gtyfokzhlq.html

set -euo pipefail
来源：http://hz.feifeiyinyue.top/gtbppqcufm.html

[R02] 变量赋值与使用
来源：http://hz.zhongyouzk.top/gtmbltqgte.html

name="Tom"; echo "$name"
来源：http://hz.jinghuilouyu.cn/gtcclwtmpd.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtdnnpflbx.html

readonly PI=3.14
来源：http://hz.sysykeji.top/gthrfwejdq.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtoamgxafm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sxryk.cn/gtficrovkj.html

[R05] 参数默认值
来源：http://hz.52xcode.cn/gtsahvbivc.html

name="${1:-default}"
来源：http://hz.gaohongyu789.top/gtfckbtwew.html

[R06] 判断命令是否存在
来源：http://hz.pengpengdd.cyou/gttdqisfsi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yanxiufei.cn/gtsihmfrxl.html

[R07] if 判断文件
来源：http://hz.c1oappe.top/gtsebmtdjl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shzxlz.cn/gtsmnjqhrd.html

[R08] 数值比较
来源：http://hz.feifeiyinyue.top/gtxvhkawvy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hnxiangtu.top/gtudltuvwg.html

[R09] 字符串比较
来源：http://hz.yonumen.top/gtnfomhekg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gotoacloud.top/gtvtgehqxz.html

[R10] 正则匹配
来源：http://hz.shanyushiyangtech.top/gtzsvfvywe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pycfn.com/gtiqcgakpa.html

[R11] case 多分支
来源：http://hz.jinqigfzy.top/gtiabbloio.html

case "$1" in
来源：http://hz.9152youxi.cn/gtknacspjj.html

start) echo "启动" ;;
来源：http://hz.cashguo.top/gtvznsrwxd.html

stop)  echo "停止" ;;
来源：http://hz.wangshuangyany.cn/gtqifczyev.html

*)     echo "未知命令" ;;
来源：http://hz.shzxlz.cn/gtkzcidjvf.html

esac
来源：http://hz.xziqi.cn/gtnovwjjsv.html

[R12] for 遍历文件
来源：http://hz.kuanghao11.cn/gtileigvsl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gtjalksphz.html

[R13] for 计数循环
来源：http://hz.jlsjyb.cn/gteamtqidq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtwdeptcqd.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gtixbzlxux.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gttyxtibwv.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtlpbuhfyd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hysaishi.cn/gtfmvuqtmi.html

[R16] until 等待条件
来源：http://hz.sufxvd.cn/gtxkyvynib.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shangyingyoupin.top/gtfhfourst.html

[R17] 数组定义与取值
来源：http://hz.hfpthk.cn/gtkvraqqyt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gttglguknf.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gtbxheofxd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.mhx1999.top/gtoufowfkb.html

[R19] 数组长度
来源：http://hz.52xcode.cn/gtacxmwxtp.html

echo "${#arr[@]}"
来源：http://hz.hfpthk.cn/gtuqmcuuwp.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtylcrjzso.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.mhx1999.top/gtmcrvcojm.html

[R21] 字符串长度
来源：http://hz.havefunace.top/gtufggmzit.html

echo "${#s}"
来源：http://hz.shuidangran.top/gtxalihjgv.html

[R22] 截取子串
来源：http://hz.yueranfly.top/gtjtzxwmid.html

echo "${s:0:5}"
来源：http://hz.9152youxi.cn/gtkjdgazrh.html

[R23] 字符串替换
来源：http://hz.nanxinkj.top/gtryotomub.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cdnleiting.top/gtsfhhgjtz.html

[R24] 大小写转换
来源：http://hz.cqqwz.cn/gtrbhmjuwc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hfpthk.cn/gtleuybsra.html

[R25] 去后缀 / 去前缀
来源：http://hz.jinqigfzy.top/gttpcfsqma.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tanke756.top/gtupqjrtvd.html

[R26] 命令替换
来源：http://hz.yuanzhike.top/gtkiuqnkkg.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtcidklhrz.html

[R27] 算术展开
来源：http://hz.yj20258888.top/gtejolqnfq.html

echo $((1 + 2 * 3))
来源：http://hz.zhijiandao.cn/gtwyssbaal.html

[R28] 浮点运算
来源：http://hz.yuxming.cn/gtvgwjjens.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtomcmmerc.html

[R29] 定义函数
来源：http://hz.pengpengdd.cyou/gtrmujsdvd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenjidiqi.icu/gtwyrtjnyu.html

[R30] 函数返回状态码
来源：http://hz.guowangkeji.top/gthksfipmd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cdnleiting.top/gtnnwyrjyu.html

[R31] 局部变量
来源：http://hz.chenzaomai.com/gtrpuzxgar.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtqilwdtoo.html

[R32] 参数个数校验
来源：http://hz.0kj1m.cn/gtwmqxsyjj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tanke756.top/gtrwarfapi.html

[R33] 捕获错误并提示行号
来源：http://hz.ehwqpu.com/gtrfraproy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuanzx.com/gtgxmvygft.html

[R34] 退出时清理
来源：http://hz.nanxuanxn.top/gtofdahunf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.fengsongda.top/gtcbdojuvn.html

[R35] 后台执行并等待
来源：http://hz.xziqi.cn/gtbifsthxh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangshuangyany.cn/gteebozzft.html

[R36] 并发执行多个任务
来源：http://hz.zhiwuduotai.top/gthecratgm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenlongwang.top/gtxipcxljs.html

[R37] 把输出赋给变量
来源：http://hz.hywenlv.cn/gtkfsljxwj.html

files=$(ls -1)
来源：http://hz.yangfankeji.com/gtwwhlflsz.html

[R38] 管道串联
来源：http://hz.yvedp.cn/gtqvxfuozg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yangfankeji.com/gtydlzltpu.html

[R39] 重定向标准输出与错误
来源：http://hz.hammf.cn/gtikddhtlh.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gteraxmbup.html

[R40] 追加写日志
来源：http://hz.andypj.xyz/gtuxqyqqgk.html

echo "log" >> out.log
来源：http://hz.hnxiangtu.top/gtkwbxetgn.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtzotgmjpk.html

cmd >/dev/null 2>&1
来源：http://hz.mhx1999.top/gtuwtbonpw.html

[R42] 输入重定向
来源：http://hz.sufxvd.cn/gteykjsnmr.html

wc -l < a.txt
来源：http://hz.jqgfzy.top/gtrzrlsxaj.html

[R43] 按名字查找文件
来源：http://hz.yj202588.top/gttlycojrd.html

find . -name "*.log" -type f
来源：http://hz.tian-w.cn/gtxhcfuuwd.html

[R44] 按修改时间查找
来源：http://hz.haohaochexian.top/gtdclwcpwh.html

find . -mtime -7 -type f
来源：http://hz.52xcode.cn/gtxvjcwbce.html

[R45] 批量删除
来源：http://hz.jinqigufen.top/gtyydeslcl.html

find . -name "*.tmp" -delete
来源：http://hz.wangshuangyany.cn/gtzukapaqw.html

[R46] 递归替换文件内容
来源：http://hz.hysaishi.cn/gtpqwfcjen.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tianlin.xyz/gteaihnoth.html

[R47] sed 单行替换
来源：http://hz.zycfv.cn/gtsfcrmspt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydjk.org.cn/gtfuckbunw.html

[R48] awk 取指定列
来源：http://hz.ybcxt.top/gttnxgohac.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxinkj.top/gtcyppwoew.html

[R49] awk 带条件
来源：http://hz.hfpthk.cn/gtfbmtyfvj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yuanzhike.top/gtrytskcvy.html

[R50] awk 求和
来源：http://hz.redwolf501.top/gtcggqrcir.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gtldgxhgxl.html

[R51] 排序去重取前几
来源：http://hz.haohaochexian.top/gtbubkecvs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhoulong.xyz/gtkhwcdubf.html

[R52] 统计行数
来源：http://hz.yanxiufei.cn/gthgzutiee.html

wc -l a.txt
来源：http://hz.hongshengwenyu.top/gtmtvnupmg.html

[R53] 查看文件头与实时尾
来源：http://hz.vqdsnc.cn/gtartsdkfg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.quarkkingdee.top/gtffmaluvo.html

[R54] 比较两个文件
来源：http://hz.xingfuxueyuan.xyz/gtvekiagbu.html

diff a.txt b.txt
来源：http://hz.316326.xyz/gtpsoeqcwv.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gtltizmmsw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.iojbl.cn/gtajzrhqfc.html

[R56] 远程拷贝
来源：http://hz.tanke756.top/gtssfeszmx.html

scp file user@host:/path/
来源：http://hz.yueranfly.top/gtbaofsggr.html

[R57] 远程执行命令
来源：http://hz.hammf.cn/gtipbsuipg.html

ssh user@host 'uptime'
来源：http://hz.9152youxi.cn/gtlyifvdds.html

[R58] 下载文件
来源：http://hz.hfpthk.cn/gtynohzlhp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258888.top/gtzsxgsuci.html

[R59] 发 POST JSON
来源：http://hz.xinyue.icu/gtainvazge.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtrmdgytvi.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtwcfvjnww.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.svipenyu.cn/gtgcceexav.html

[R61] 磁盘占用
来源：http://hz.shzxlz.cn/gtroaxdzqt.html

df -h;  du -sh *
来源：http://hz.havefunace.top/gtnmkzrlpw.html

[R62] 找最占空间的文件
来源：http://hz.yanxiufei.cn/gtogefuurr.html

du -ah . | sort -rh | head -10
来源：http://hz.ivvv.top/gtjagiwxok.html

[R63] 内存与进程
来源：http://hz.zycfv.cn/gtwguordci.html

free -h;  ps aux | grep nginx
来源：http://hz.ydjk.org.cn/gtvgakwhvx.html

[R64] 结束进程
来源：http://hz.shzxlz.cn/gtvemtvngj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtqrhusxlt.html

[R65] 查看端口占用
来源：http://hz.hammf.cn/gtcgvsxjzo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.birdmap.top/gtvfoewdpk.html

[R66] 定时任务
来源：http://hz.aibaodan.cn/gtmddwpmpc.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtnlaiusvd.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtuqxtsoti.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gttyvybckl.html

[R68] 计算文件校验值
来源：http://hz.yanxiufei.cn/gthjrpuxvx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hysaishi.cn/gtjnxmprfn.html

[R69] 生成随机密码
来源：http://hz.daria6918.cn/gthhvhqofj.html

head -c 16 /dev/urandom | base64
来源：http://hz.sweek.top/gtkefmnsog.html

[R70] 时间戳与互转
来源：http://hz.yuanzhike.top/gtkldfhjgq.html

date +%s;  date -d @1700000000
来源：http://hz.jlsjyb.cn/gtxwomvwbt.html

[R71] 日期格式化
来源：http://hz.shuidangran.top/gteycloacv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xziqi.cn/gtcdrzuosn.html

[R72] 等待端口就绪
来源：http://hz.ydzc1.top/gtfvmakbhj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jqgufenzy.top/gthogpnffb.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gtkfimbalw.html

split -l 1000 big.log part_
来源：http://hz.yj20258888.top/gtsmqjjprs.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtlnhzplda.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gtlioeeosm.html

[R75] 导出环境变量
来源：http://hz.yonumen.top/gtbniwyqsi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daxiang520.top/gtejrrjckp.html

[R76] 使用临时文件
来源：http://hz.daxiang520.top/gtthtbwplw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtmnbvxrwq.html

[R77] 读取用户输入
来源：http://hz.zdqjudy.top/gtwkqzgvsu.html

read -rp "请输入: " ans
来源：http://hz.dianchejie.cn/gtxqkhouee.html

[R78] 交互式菜单
来源：http://hz.ivvv.top/gtkxtbksmg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.smart0.xyz/gtokjvbdew.html

[R79] 解析命令行选项
来源：http://hz.aizwys.cn/gtpcfudspv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gtinmkoonl.html

[R80] 查看脚本执行耗时
来源：http://hz.feifeiyinyue.top/gtvgyyvjye.html

time ./run.sh
来源：http://hz.jyoumei.cn/gtwzzoycxi.html

================================================================================
来源：http://hz.yuxming.cn/gtvgatelad.html

S. C / C++ 专题
来源：http://hz.yj20258.top/gtwbxrayup.html

================================================================================
来源：http://hz.zdqjudy.top/gtumvrnuta.html

[S01] C：Hello World
来源：http://hz.316326.xyz/gtaepapsmy.html

#include <stdio.h>
来源：http://hz.zhoulong.xyz/gtpiiilonc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sweek.top/gtuhchuuby.html

[S02] C：变量与格式化输出
来源：http://hz.haohaochexian.top/gtdaaesmxq.html

int a = 10; printf("%d\n", a);
来源：http://hz.c1oappe.top/gtzkjdtoua.html

[S03] C：读入整数
来源：http://hz.sysykeji.top/gtylokflwx.html

int x; scanf("%d", &x);
来源：http://hz.ybcxt.top/gtbmkfrbvc.html

[S04] C：字符串复制
来源：http://hz.xingfuxueyuan.xyz/gthomklxqo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.vqdsnc.cn/gtamyjooxs.html

[S05] C：字符串长度
来源：http://hz.yangfankeji.com/gtxcnmvmpl.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtbgpfswlj.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gtseyrfxdv.html

strcmp(a, b) == 0
来源：http://hz.yj202588.top/gtmhaboyqe.html

[S07] C：数组遍历求和
来源：http://hz.tian-w.cn/gtrnqgnghq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aibaodan.cn/gttmhwqqvl.html

[S08] C：动态内存分配与释放
来源：http://hz.feifeiyinyue.top/gtwpatlhwg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jqgfzy.top/gteirzlfbd.html

[S09] C：结构体定义与初始化
来源：http://hz.ydjk.org.cn/gtmsqaaffw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj20258888.top/gtwjqyornm.html

[S10] C：指针与解引用
来源：http://hz.ydjk.org.cn/gtmvaeobns.html

int *p = &a;  *p = 5;
来源：http://hz.yangfankeji.com/gtzstgjufd.html

[S11] C：逐行读文件
来源：http://hz.meibo888.top/gtgegxmvfw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daxiang520.top/gtlfofhtqj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jianghu66.top/gtglaokham.html

fclose(f);
来源：http://hz.fzhhl.top/gtoxyogqxf.html

[S12] C：写文件
来源：http://hz.haohaochexian.top/gtuzifrotg.html


<!-- 参考信息 -->