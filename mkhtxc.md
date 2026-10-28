代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hz.zhixingplan.top/gtydlbrfed.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hnqzz.top/gtawhisucm.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtxuhefahc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.smart0.xyz/gthjbzzlkz.html

[Q44] IN 子查询
来源：http://hz.c1oappe.top/gtcthlyyaa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sysykeji.top/gtcvyfkdsp.html

[Q45] EXISTS 判断存在
来源：http://hz.hnqzz.top/gtlyrjmxjy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gteebvcpwc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gtlareylry.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtfmzfsuhw.html

[Q47] 与平均值比较
来源：http://hz.yj202588.top/gtdocmtvhb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gtdbitvfcr.html

[Q48] CTE 公用表表达式
来源：http://hz.mhx1999.top/gtwxfmowts.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhijiandao.cn/gtumvkfsgm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hfpthk.cn/gtsjesiknw.html

[Q49] 更新单行
来源：http://hz.yuxming.cn/gtsrshiyjj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtepkpupki.html

[Q50] 批量更新
来源：http://hz.jlsjyb.cn/gtlbfqgdwr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shanyushiyangtech.top/gthcdmbker.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtpipdvpuy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.feifeiyinyue.top/gtleknbedd.html

[Q52] 删除指定行
来源：http://hz.cashguo.top/gtrqkgqhjj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtqtfbzyhs.html

[Q53] 按条件删除
来源：http://hz.aibaodan.cn/gtweezbjbs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cheryme.top/gtweezybin.html

[Q54] 清空表
来源：http://hz.yangfankeji.com/gthwptrenw.html

TRUNCATE TABLE logs;
来源：http://hz.zhijiandao.cn/gtcaxlbmxp.html

[Q55] 排名（并列占位）
来源：http://hz.ehwqpu.com/gtpvfjywif.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gzhubu.top/gttbycmkkh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yonumen.top/gtvbrhqdmb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aizwys.cn/gtserdrpqb.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtacxnogex.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.andypj.xyz/gtucckeqjf.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gtvdiwbdsb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.snrcjt.cn/gtvtokzelj.html

[Q59] 分组内累计
来源：http://hz.xuanzx.com/gtkjzrbnsj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxuanxn.top/gtqmumvyfs.html

[Q60] 取上一行 / 下一行
来源：http://hz.jianghu66.top/gtwosrehjo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ywan-chungtsiang.top/gtkanrhets.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtuwaqzbwg.html

[Q61] 移动平均
来源：http://hz.jqgufenzy.top/gtxnyjojow.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.havefunace.top/gtgpcjpguc.html

[Q62] 分组占比
来源：http://hz.gaohongyu789.top/gtnofahmso.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtzpstlwsj.html

[Q63] 开启事务
来源：http://hz.smart0.xyz/gtfcjcygqa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenjidiqi.icu/gtxibcimpm.html

[Q64] 提交事务
来源：http://hz.tanke756.top/gtjhaiidza.html

COMMIT;
来源：http://hz.pycfn.com/gtwmrhzwzl.html

[Q65] 回滚事务
来源：http://hz.hongshengwenyu.top/gthiczdqvu.html

ROLLBACK;
来源：http://hz.xingfuxueyuan.xyz/gtxbgzanic.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gtcieijfkv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.svipenyu.cn/gtvontysfe.html

[Q67] 设置隔离级别
来源：http://hz.xuetiantiany.cn/gtodpvzgdj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gogol.net.cn/gtnrlvsutz.html

[Q68] 保存点
来源：http://hz.cucudq.cn/gtljwvfatu.html

SAVEPOINT sp1;
来源：http://hz.yj202588.top/gtoojufsjy.html

ROLLBACK TO sp1;
来源：http://hz.cheryme.top/gtdeucrfza.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtuhvymimj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj202588.top/gtdszbmfet.html

[Q70] 更新统计信息
来源：http://hz.xuanzx.com/gtvufedgwa.html

ANALYZE TABLE users;
来源：http://hz.smart0.xyz/gtmxjtftvk.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtwjcsqkze.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnxiangtu.top/gtxjhlyavh.html

[Q72] 查看索引
来源：http://hz.zhengqikj.top/gtoebvxlkf.html

SHOW INDEX FROM users;
来源：http://hz.yj20258888.top/gtiqpooldp.html

[Q73] 查看表状态
来源：http://hz.sysykeji.top/gtsecpgfdj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yvedp.cn/gtdkrrfund.html

[Q74] 强制使用索引
来源：http://hz.ehwqpu.com/gtrtyplanc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.bjfxy.top/gtxozbbxoh.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtmtfhaqss.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.meibo888.top/gtqkybocfp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sweek.top/gtaohctqnz.html

[Q76] 按天统计
来源：http://hz.jqgfzy.top/gtoxhaqoyn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangdashe.top/gtyvwisysw.html

[Q77] 时间加减
来源：http://hz.chenlongwang.top/gtrqenowdt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jiagoushi.top/gttoohjhdg.html

[Q78] 当前时间
来源：http://hz.ydjk.org.cn/gtkbwsuwjy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sweek.top/gtmheqcvkz.html

[Q79] 字符串拼接
来源：http://hz.xinyue.icu/gtgewmdqjy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhengqikj.top/gtuaskqeot.html

[Q80] 字符串截取
来源：http://hz.dianchejie.cn/gtdygxrppk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xinyue.icu/gtnpebtrkp.html

[Q81] 字符串替换
来源：http://hz.quarkkingdee.top/gtslkwkpvs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jyoumei.cn/gtapzffdlc.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gtpmlbybzr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtswqonywk.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtwvdmront.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.vqdsnc.cn/gthtisofxy.html

[Q84] 去除首尾空格
来源：http://hz.hongshengwenyu.top/gtrswdvuqc.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhongyouzk.top/gtlqzicsbf.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtwpwperjw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aizwys.cn/gtqrnnxgob.html

[Q86] 读取 JSON 字段
来源：http://hz.ywan-chungtsiang.top/gtgwvvyrtc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jqgfzy.top/gthnruplcl.html

[Q87] JSON 字段做条件
来源：http://hz.cqqwz.cn/gtybvusfwx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.iojbl.cn/gtwkocilwh.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigfzy.top/gtfolqytar.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jyoumei.cn/gtqlswtepp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnqzz.top/gtizaxeacs.html

[Q89] 判断表是否存在
来源：http://hz.havefunace.top/gtazcandnt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.wangshuangyany.cn/gtcmxfuyom.html

[Q90] 生成序号列
来源：http://hz.xuetiantiany.cn/gtcrqosikg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tanke756.top/gtezftbpwy.html

================================================================================
来源：http://hz.snrcjt.cn/gtdoqepvsh.html

R. Bash 专题
来源：http://hz.yj20258.top/gtstfomdem.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmfurqlmm.html

[R01] shebang 与严格模式
来源：http://hz.xylfe.cn/gtgtogqiex.html

#!/usr/bin/env bash
来源：http://hz.daria6918.cn/gtfotrxvnd.html

set -euo pipefail
来源：http://hz.ehwqpu.com/gttucyhunf.html

[R02] 变量赋值与使用
来源：http://hz.c1oappe.top/gtnvshcjvv.html

name="Tom"; echo "$name"
来源：http://hz.wangdashe.top/gtpytduomu.html

[R03] 只读变量
来源：http://hz.ywan-chungtsiang.top/gtrlkcupmw.html

readonly PI=3.14
来源：http://hz.bjfxy.top/gtxtymxxbq.html

[R04] 位置参数
来源：http://hz.ppjwa.cn/gthavhckhp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhoulong.xyz/gtargvscda.html

[R05] 参数默认值
来源：http://hz.guowangkeji.top/gtnccvyyvc.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtzpwvkxgx.html

[R06] 判断命令是否存在
来源：http://hz.zycfv.cn/gtgqvrgiru.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gttitimqhm.html

[R07] if 判断文件
来源：http://hz.yj20258888.top/gtfaeaaonr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhixingplan.top/gtnyxkbwnm.html

[R08] 数值比较
来源：http://hz.gotoacloud.top/gtoawvraoi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.0kj1m.cn/gtkbhxbzpq.html

[R09] 字符串比较
来源：http://hz.cheryme.top/gtgmhgtpwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yangfankeji.com/gtiprbukjr.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtbtlhqqfv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtkxnesnav.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gtblqpkbqy.html

case "$1" in
来源：http://hz.316326.xyz/gtllnnnxhn.html

start) echo "启动" ;;
来源：http://hz.meibo888.top/gtlijmfoux.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtlnozotfp.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtmrgipcqz.html

esac
来源：http://hz.zhoulong.xyz/gtaxiumxlz.html

[R12] for 遍历文件
来源：http://hz.cheryme.top/gtvkbshjjf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258.top/gtmuhsejkq.html

[R13] for 计数循环
来源：http://hz.jiagoushi.top/gtovwdguof.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtetoqnuwn.html

[R14] C 风格 for
来源：http://hz.52xcode.cn/gtfaoqlumz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daria6918.cn/gtnqhtccbm.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtmusfjwdd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gaohongyu789.top/gtfyhqzmhg.html

[R16] until 等待条件
来源：http://hz.xylfe.cn/gtvqvvycza.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cashguo.top/gtbltuhxnw.html

[R17] 数组定义与取值
来源：http://hz.tianlin.xyz/gtjzipwueg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sxryk.cn/gtqjztagah.html

[R18] 遍历数组
来源：http://hz.yvedp.cn/gtrusgrayi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.dianchejie.cn/gtkhpqttsh.html

[R19] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtyqfecdsj.html

echo "${#arr[@]}"
来源：http://hz.shzxlz.cn/gtvyqgozss.html

[R20] 关联数组（字典）
来源：http://hz.nwbrower.top/gtcfftymik.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gtsinpqtwz.html

[R21] 字符串长度
来源：http://hz.yueranfly.top/gtuvluvtyt.html

echo "${#s}"
来源：http://hz.jlsjyb.cn/gtrowvtynr.html

[R22] 截取子串
来源：http://hz.snrcjt.cn/gtktwdcdhp.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gtirtjcocs.html

[R23] 字符串替换
来源：http://hz.mhx1999.top/gtchdjmsvy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shzxlz.cn/gtoyuiktag.html

[R24] 大小写转换
来源：http://hz.ybcxt.top/gtikfnviay.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xylfe.cn/gtqndqfhqk.html

[R25] 去后缀 / 去前缀
来源：http://hz.ybcxt.top/gtobdksuth.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.daria6918.cn/gtyozweiay.html

[R26] 命令替换
来源：http://hz.chenlongwang.top/gtpokyhkls.html

now=$(date +%F); echo "$now"
来源：http://hz.jiagoushi.top/gtownxlgpl.html

[R27] 算术展开
来源：http://hz.xingfuxueyuan.xyz/gtjrxhjmkx.html

echo $((1 + 2 * 3))
来源：http://hz.9152youxi.cn/gtvrafgzsp.html

[R28] 浮点运算
来源：http://hz.gogol.net.cn/gtvgxsaoxp.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhengqikj.top/gtggleflph.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gtusxjkjud.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ivvv.top/gtsswhxqoe.html

[R30] 函数返回状态码
来源：http://hz.xingfuxueyuan.xyz/gtsylrhkvn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ybcxt.top/gtzsaxhcsn.html

[R31] 局部变量
来源：http://hz.hywenlv.cn/gtitbwsmyn.html

f() { local x=1; echo "$x"; }
来源：http://hz.havefunace.top/gtcxpslyac.html

[R32] 参数个数校验
来源：http://hz.vqdsnc.cn/gtrikcjmjm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtiiijfdiv.html

[R33] 捕获错误并提示行号
来源：http://hz.guowangkeji.top/gtlqxqxrxa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.redwolf501.top/gtvolvtiwt.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gtqmetvkmh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gthlcjxxro.html

[R35] 后台执行并等待
来源：http://hz.hfpthk.cn/gtusjmrdit.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gtabonbrja.html

[R36] 并发执行多个任务
来源：http://hz.fengsongda.top/gtwuayghaf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guannengcc.top/gtvowrfhum.html

[R37] 把输出赋给变量
来源：http://hz.vqdsnc.cn/gtntrvgjti.html

files=$(ls -1)
来源：http://hz.hywenlv.cn/gtobuxqudg.html

[R38] 管道串联
来源：http://hz.daxiang520.top/gtvdkqfkmc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nwbrower.top/gtalwrmfwe.html

[R39] 重定向标准输出与错误
来源：http://hz.cdnleiting.top/gtqdrjvqbu.html

cmd > out.log 2>&1
来源：http://hz.guowangkeji.top/gtrlwmgjec.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtrdheiund.html

echo "log" >> out.log
来源：http://hz.hfpthk.cn/gtuvqnmtny.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gtjryxswra.html

cmd >/dev/null 2>&1
来源：http://hz.cheryme.top/gtoukvdcgg.html

[R42] 输入重定向
来源：http://hz.c1oappe.top/gtwqgzxwjo.html

wc -l < a.txt
来源：http://hz.jyoumei.cn/gtkdhkczob.html

[R43] 按名字查找文件
来源：http://hz.nanxuanxn.top/gtngfgjrxv.html

find . -name "*.log" -type f
来源：http://hz.chenjidiqi.icu/gtcckqkylt.html

[R44] 按修改时间查找
来源：http://hz.xziqi.cn/gtdqqshyyi.html

find . -mtime -7 -type f
来源：http://hz.dashuyun.cn/gtczghljvk.html

[R45] 批量删除
来源：http://hz.jinqigufen.top/gtuffahmee.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtpyofqhvl.html

[R46] 递归替换文件内容
来源：http://hz.xuanzx.com/gtnbcshtsr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.vqdsnc.cn/gtvcllwmtg.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gtttlyosah.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuanzx.com/gtnhkxcaan.html

[R48] awk 取指定列
来源：http://hz.nanxinkj.top/gtcitkdurk.html

awk '{print $1, $3}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtdqpdqpmu.html

[R49] awk 带条件
来源：http://hz.zhiwuduotai.top/gtenjldury.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gtykigzrhn.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtxrbyagdc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jqgfzy.top/gtkmdqvkqa.html

[R51] 排序去重取前几
来源：http://hz.jinqigfzy.top/gttblvxinq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shangyingyoupin.top/gtcjxgufuw.html

[R52] 统计行数
来源：http://hz.kuanghao11.cn/gtzhaxoqdd.html

wc -l a.txt
来源：http://hz.hnxiangtu.top/gturkzlufk.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gtbvjmlatb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtrdfukwuz.html

[R54] 比较两个文件
来源：http://hz.svipenyu.cn/gtlyxjehvh.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtmkhfyxqg.html

[R55] 压缩与解压
来源：http://hz.zhoulong.xyz/gthbhuelmr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sysykeji.top/gtznsdpuwr.html

[R56] 远程拷贝
来源：http://hz.jqgfzy.top/gtutrpzhts.html

scp file user@host:/path/
来源：http://hz.yj20258.top/gtcnmjzfhw.html

[R57] 远程执行命令
来源：http://hz.zhoulong.xyz/gtuigyjcet.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtdzirdqel.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gtzvsxxlit.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhoulong.xyz/gtlcqzwpxa.html

[R59] 发 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtebryjart.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtzicozpcm.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtzqlecued.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.0kj1m.cn/gtntgmtagc.html

[R61] 磁盘占用
来源：http://hz.0kj1m.cn/gtravnkwyj.html

df -h;  du -sh *
来源：http://hz.wangshuangyany.cn/gtsamxidqn.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtpgnqkumy.html

du -ah . | sort -rh | head -10
来源：http://hz.snrcjt.cn/gtbcyitzhq.html

[R63] 内存与进程
来源：http://hz.sweek.top/gtsbwdjabw.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtirbgzecs.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtcqyiylne.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sweek.top/gtluvysdbw.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtybzadosu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dashuyun.cn/gtrbqclumd.html

[R66] 定时任务
来源：http://hz.smart0.xyz/gtzywuajzh.html

crontab -e;  crontab -l
来源：http://hz.hammf.cn/gtiixrffrx.html

[R67] 生成随机十六进制串
来源：http://hz.9152youxi.cn/gtolajeitb.html

openssl rand -hex 16
来源：http://hz.aizwys.cn/gtbnjcovlp.html

[R68] 计算文件校验值
来源：http://hz.hfpthk.cn/gtygqeishl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aizwys.cn/gtodqjqnbr.html

[R69] 生成随机密码
来源：http://hz.yuanzhike.top/gtvpdguvwg.html

head -c 16 /dev/urandom | base64
来源：http://hz.tanke756.top/gtxbtefaag.html

[R70] 时间戳与互转
来源：http://hz.shangyingyoupin.top/gtvjpnqxvj.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtiahhcsba.html

[R71] 日期格式化
来源：http://hz.nwbrower.top/gtbsqkmkil.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cucudq.cn/gtzungxsdw.html

[R72] 等待端口就绪
来源：http://hz.redwolf501.top/gtobkmrvqk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtshwzchib.html

[R73] 分割大日志
来源：http://hz.hammf.cn/gtuqowomei.html

split -l 1000 big.log part_
来源：http://hz.birdmap.top/gtddthlspr.html

[R74] 批量重命名
来源：http://hz.havefunace.top/gthfnmnlkz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hongshengwenyu.top/gttevkznsc.html

[R75] 导出环境变量
来源：http://hz.cdnleiting.top/gtmopjirfq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gtfjnjghmv.html

[R76] 使用临时文件
来源：http://hz.cucudq.cn/gtulrngbxs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtadcgmzyp.html

[R77] 读取用户输入
来源：http://hz.xziqi.cn/gtpvkqifve.html

read -rp "请输入: " ans
来源：http://hz.aizwys.cn/gtzjoxppay.html

[R78] 交互式菜单
来源：http://hz.xylfe.cn/gtsxbnnagi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cucudq.cn/gtuqblcqgw.html

[R79] 解析命令行选项
来源：http://hz.hongshengwenyu.top/gtaovprhvw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydzc1.top/gtegwliuxe.html

[R80] 查看脚本执行耗时
来源：http://hz.chenzaomai.com/gticuopeif.html

time ./run.sh
来源：http://hz.yanxiufei.cn/gtxahqvhss.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtrwfnluuy.html

S. C / C++ 专题
来源：http://hz.ydzc1.top/gtmwrqpapz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqnswrhkp.html

[S01] C：Hello World
来源：http://hz.jqgufenzy.top/gtbtyedqdl.html

#include <stdio.h>
来源：http://hz.xuetiantiany.cn/gthwazdysj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj20258888.top/gtkslcspbg.html

[S02] C：变量与格式化输出
来源：http://hz.jinqigufen.top/gtobaalcrn.html

int a = 10; printf("%d\n", a);
来源：http://hz.pengpengdd.cyou/gtpbvrekie.html

[S03] C：读入整数
来源：http://hz.gogol.net.cn/gtcywcjdff.html

int x; scanf("%d", &x);
来源：http://hz.jiagoushi.top/gtiyqdycvv.html

[S04] C：字符串复制
来源：http://hz.snrcjt.cn/gtcsyujxxh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnxiangtu.top/gtiejacmmu.html

[S05] C：字符串长度
来源：http://hz.jiagoushi.top/gthrqwgxyx.html

strlen(s)
来源：http://hz.zycfv.cn/gtvmktyzlq.html

[S06] C：字符串比较
来源：http://hz.ybcxt.top/gtxoksaixf.html

strcmp(a, b) == 0
来源：http://hz.guannengcc.top/gttejfknte.html

[S07] C：数组遍历求和
来源：http://hz.ivvv.top/gtiamtakmy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gogol.net.cn/gtdswytptu.html

[S08] C：动态内存分配与释放
来源：http://hz.gzhubu.top/gtiylzuron.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dashuyun.cn/gtehhhwmdg.html

[S09] C：结构体定义与初始化
来源：http://hz.iojbl.cn/gtnaufhmrx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xylfe.cn/gtzhwlgnhc.html

[S10] C：指针与解引用
来源：http://hz.jinghuilouyu.cn/gtrdzcuxma.html

int *p = &a;  *p = 5;
来源：http://hz.sufxvd.cn/gteghsrlmo.html

[S11] C：逐行读文件
来源：http://hz.jlsjyb.cn/gtdiqtokxn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtkaejwcma.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhijiandao.cn/gtvmndgoeh.html

fclose(f);
来源：http://hz.hongshengwenyu.top/gtgenylfln.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gtdkgopxnc.html


<!-- 参考信息 -->