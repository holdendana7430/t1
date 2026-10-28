代发 wailian999

[Q44] IN 子查询
来源：http://hz.9152youxi.cn/gtxxvghqob.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtnsuydzps.html

[Q45] EXISTS 判断存在
来源：http://hz.xziqi.cn/gtzrqolcqs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sweek.top/gtfymylsui.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtskttgphi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtkuiztbcn.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtsblmxxmv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sweek.top/gtcqfjcdyj.html

[Q48] CTE 公用表表达式
来源：http://hz.aizwys.cn/gtpapoamic.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cdnleiting.top/gtdxqcopbk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.birdmap.top/gtzqgdyrsm.html

[Q49] 更新单行
来源：http://hz.ywan-chungtsiang.top/gtbcyqedem.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yongpay.top/gtcrxhapex.html

[Q50] 批量更新
来源：http://hz.zhongyouzk.top/gtglntdzth.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gotoacloud.top/gtgqqncysl.html

[Q51] 用子查询更新
来源：http://hz.hnqzz.top/gtdqmuyghz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gtlimwzema.html

[Q52] 删除指定行
来源：http://hz.birdmap.top/gthcrftdfz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhiwuduotai.top/gtcbryulxx.html

[Q53] 按条件删除
来源：http://hz.andypj.xyz/gtfgoxokmm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtvwcznwxs.html

[Q54] 清空表
来源：http://hz.ehwqpu.com/gtoikycocl.html

TRUNCATE TABLE logs;
来源：http://hz.vqdsnc.cn/gtjksiljfm.html

[Q55] 排名（并列占位）
来源：http://hz.chenlongwang.top/gtckzynnqh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hammf.cn/gtnciyklgm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.c1oappe.top/gtxmiojwet.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.guowangkeji.top/gtfhslcewz.html

[Q57] 行号
来源：http://hz.hfpthk.cn/gtihukwzqn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shzxlz.cn/gtnqpkpbhq.html

[Q58] 累计求和
来源：http://hz.zhijiandao.cn/gtldmsfeby.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tianlin.xyz/gtpinqsvbn.html

[Q59] 分组内累计
来源：http://hz.zhiwuduotai.top/gtljeamxzx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gaohongyu789.top/gtrhbffblx.html

[Q60] 取上一行 / 下一行
来源：http://hz.zycfv.cn/gtqmihgmvj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gtzdssyznm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtzevpoboo.html

[Q61] 移动平均
来源：http://hz.ehwqpu.com/gttvqqoezy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtpglohdug.html

[Q62] 分组占比
来源：http://hz.vqdsnc.cn/gthpbqycox.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtpyprzyxx.html

[Q63] 开启事务
来源：http://hz.vqdsnc.cn/gtwheupwmv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yanxiufei.cn/gtijwqvgbr.html

[Q64] 提交事务
来源：http://hz.cdnleiting.top/gtvbcjjryk.html

COMMIT;
来源：http://hz.wangshuangyany.cn/gtwhnnnfoj.html

[Q65] 回滚事务
来源：http://hz.ywan-chungtsiang.top/gtnxmlsdpq.html

ROLLBACK;
来源：http://hz.tanke756.top/gtszybjpqd.html

[Q66] 行锁查询
来源：http://hz.cdnleiting.top/gthnbzdoch.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258.top/gtylzhuzgg.html

[Q67] 设置隔离级别
来源：http://hz.zhijiandao.cn/gtoarzgcdx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.andypj.xyz/gthculrtat.html

[Q68] 保存点
来源：http://hz.0kj1m.cn/gtzhlnniks.html

SAVEPOINT sp1;
来源：http://hz.xylfe.cn/gthgsvitwi.html

ROLLBACK TO sp1;
来源：http://hz.tianlin.xyz/gtkdohjfin.html

[Q69] 查看执行计划
来源：http://hz.ybcxt.top/gtbdyucajo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.dashuyun.cn/gtqbkyuwaw.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gtgucqsifw.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangtech.top/gtkwisdiqx.html

[Q71] 查看建表语句
来源：http://hz.hongshengwenyu.top/gtsepsugrf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtoewrrlsr.html

[Q72] 查看索引
来源：http://hz.guowangkeji.top/gtsmfzkfer.html

SHOW INDEX FROM users;
来源：http://hz.feifeiyinyue.top/gtmkamrgim.html

[Q73] 查看表状态
来源：http://hz.yj20258888.top/gtohsxpcec.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cheryme.top/gtaezxnruu.html

[Q74] 强制使用索引
来源：http://hz.wangshuangyany.cn/gtnkxyklps.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhiwuduotai.top/gtfgmkysjq.html

[Q75] 日期格式化
来源：http://hz.daria6918.cn/gtizfbikoa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yangfankeji.com/gtsafsijgn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydjk.org.cn/gtbdgxssxj.html

[Q76] 按天统计
来源：http://hz.xuetiantiany.cn/gtfygrcrlo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.feifeiyinyue.top/gtcbezzgcd.html

[Q77] 时间加减
来源：http://hz.dashuyun.cn/gtcsyebodx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dianchejie.cn/gtczkxkers.html

[Q78] 当前时间
来源：http://hz.fzhhl.top/gthtpaoiry.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.kuanghao11.cn/gtknplclmy.html

[Q79] 字符串拼接
来源：http://hz.yuxming.cn/gtrbmtcjdy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.mhx1999.top/gtsgfxfivm.html

[Q80] 字符串截取
来源：http://hz.sufxvd.cn/gtgfpqyjhx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.bjfxy.top/gtccwkjtqf.html

[Q81] 字符串替换
来源：http://hz.zhongyouzk.top/gtqqczrkwk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtchfyufwa.html

[Q82] 字符长度与字节长度
来源：http://hz.yueranfly.top/gttjsupfmx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtwkpoxpae.html

[Q83] 大小写转换
来源：http://hz.zhiwuduotai.top/gtngynfxla.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xinyue.icu/gtlqqslicj.html

[Q84] 去除首尾空格
来源：http://hz.aibaodan.cn/gtrbgqqhpj.html

SELECT TRIM(name) FROM users;
来源：http://hz.shuidangran.top/gtyyxwrzun.html

[Q85] 数值取整
来源：http://hz.52xcode.cn/gtaufqgogn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigufen.top/gtfsxzzhds.html

[Q86] 读取 JSON 字段
来源：http://hz.aizwys.cn/gtpkfuyibx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gtubtvctlx.html

[Q87] JSON 字段做条件
来源：http://hz.zhijiandao.cn/gtcumsviuw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ybcxt.top/gtgbgjfqtf.html

[Q88] 行转列（条件聚合）
来源：http://hz.0kj1m.cn/gthlqcslru.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gteemlgsqc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtihnvnamj.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gtthqcpsun.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gtgjmqggrv.html

[Q90] 生成序号列
来源：http://hz.sysykeji.top/gtzsoeifap.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gtsrgwzaej.html

================================================================================
来源：http://hz.gogol.net.cn/gteuencxlf.html

R. Bash 专题
来源：http://hz.0kj1m.cn/gtkjuffqrt.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrajyzprl.html

[R01] shebang 与严格模式
来源：http://hz.guannengcc.top/gtqdymhurm.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtnxwwyryt.html

set -euo pipefail
来源：http://hz.sysykeji.top/gtmyujdbfr.html

[R02] 变量赋值与使用
来源：http://hz.zhoulong.xyz/gtebtvlfsh.html

name="Tom"; echo "$name"
来源：http://hz.yanxiufei.cn/gtwxzplfdj.html

[R03] 只读变量
来源：http://hz.iojbl.cn/gtjfhktppw.html

readonly PI=3.14
来源：http://hz.0kj1m.cn/gtjzrwrjbo.html

[R04] 位置参数
来源：http://hz.sweek.top/gtrfhcvsrg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.316326.xyz/gtptqnakao.html

[R05] 参数默认值
来源：http://hz.zhengqikj.top/gtsktdiqdp.html

name="${1:-default}"
来源：http://hz.meibo888.top/gtslhjjccu.html

[R06] 判断命令是否存在
来源：http://hz.zhixingplan.top/gthmtzdrag.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigufen.top/gtxqiimcky.html

[R07] if 判断文件
来源：http://hz.guannengcc.top/gtinlkparg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aizwys.cn/gtzgenaaku.html

[R08] 数值比较
来源：http://hz.pycfn.com/gtiejbzajg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tanke756.top/gtexxhhjhj.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtdoqbdkuu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinqigufen.top/gtuqqlkxvc.html

[R10] 正则匹配
来源：http://hz.jqgfzy.top/gtozjulcfe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hongshengwenyu.top/gtekfonjay.html

[R11] case 多分支
来源：http://hz.52xcode.cn/gtzvutxoug.html

case "$1" in
来源：http://hz.nanxuanxn.top/gtbbhnynux.html

start) echo "启动" ;;
来源：http://hz.hnxiangtu.top/gtptfnnmad.html

stop)  echo "停止" ;;
来源：http://hz.xylfe.cn/gtyzqysfyp.html

*)     echo "未知命令" ;;
来源：http://hz.wangshuangyany.cn/gtnpkubhfj.html

esac
来源：http://hz.c1oappe.top/gtwujlxdhs.html

[R12] for 遍历文件
来源：http://hz.jinqigufen.top/gthwiobpdk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhaomingkeji.xyz/gtmlwbsveq.html

[R13] for 计数循环
来源：http://hz.xuetiantiany.cn/gtxpkxfbwc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtngupmwdw.html

[R14] C 风格 for
来源：http://hz.fengsongda.top/gthbgfofut.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtszlvmcri.html

[R15] while 逐行读文件
来源：http://hz.cashguo.top/gtkgtucwga.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtqtrkqaum.html

[R16] until 等待条件
来源：http://hz.birdmap.top/gtuzuczdob.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtvzjezjux.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gtgpqcajbk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cashguo.top/gtkzyxkdwy.html

[R18] 遍历数组
来源：http://hz.ywan-chungtsiang.top/gtstyofupc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenjidiqi.icu/gtlerugfno.html

[R19] 数组长度
来源：http://hz.zhiwuduotai.top/gtejynbnpp.html

echo "${#arr[@]}"
来源：http://hz.yonumen.top/gturzhjmsh.html

[R20] 关联数组（字典）
来源：http://hz.zhijiandao.cn/gtcxwluucq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.9152youxi.cn/gtlxqzqirn.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtqagklmnl.html

echo "${#s}"
来源：http://hz.chenzaomai.com/gtafdvytoi.html

[R22] 截取子串
来源：http://hz.aizwys.cn/gtfqvkobfm.html

echo "${s:0:5}"
来源：http://hz.tanke756.top/gtursjoezd.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtsambaahz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.pengpengdd.cyou/gtoxbtbjcb.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gtbagmkmjd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yvedp.cn/gtqeyqdtfr.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258.top/gtobpjvlfj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigfzy.top/gtobylpzre.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gtnvgrfrdi.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gtmzmnsniz.html

[R27] 算术展开
来源：http://hz.snrcjt.cn/gtbrfxdjyj.html

echo $((1 + 2 * 3))
来源：http://hz.yj202588.top/gtnmqcycdm.html

[R28] 浮点运算
来源：http://hz.aizwys.cn/gtvpztfxhi.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtdvpaxpjk.html

[R29] 定义函数
来源：http://hz.bjfxy.top/gtuugmxnuf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuanzx.com/gtngnrwbgl.html

[R30] 函数返回状态码
来源：http://hz.fzhhl.top/gtfowbpxwd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.shanyushiyangtech.top/gtsoesvcfm.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtvxvseizw.html

f() { local x=1; echo "$x"; }
来源：http://hz.dianchejie.cn/gtyxxszmja.html

[R32] 参数个数校验
来源：http://hz.c1oappe.top/gtzntwwqlb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.vqdsnc.cn/gtsghbxyet.html

[R33] 捕获错误并提示行号
来源：http://hz.zhijiandao.cn/gtwxgjfwvd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.birdmap.top/gtiuagoorw.html

[R34] 退出时清理
来源：http://hz.pengpengdd.cyou/gtgxpkdnyi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgufenzy.top/gtvbmyaqkw.html

[R35] 后台执行并等待
来源：http://hz.chenjidiqi.icu/gtnsnmkurf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cdnleiting.top/gtmwiiangn.html

[R36] 并发执行多个任务
来源：http://hz.jiagoushi.top/gtrdgfhfly.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jiagoushi.top/gtckduiwci.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gtkyewqgdz.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtbnxmnzjx.html

[R38] 管道串联
来源：http://hz.shanyushiyangtech.top/gtuwcuahbz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtwvjgqzsa.html

[R39] 重定向标准输出与错误
来源：http://hz.hfpthk.cn/gtukasyfnr.html

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtfszesgyy.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtingnjcfw.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtjdmpnvko.html

[R41] 丢弃输出
来源：http://hz.hnxiangtu.top/gtiasbpavi.html

cmd >/dev/null 2>&1
来源：http://hz.sufxvd.cn/gtlubiawoy.html

[R42] 输入重定向
来源：http://hz.xuanzx.com/gtwcdjzblr.html

wc -l < a.txt
来源：http://hz.hywenlv.cn/gtybfvamcc.html

[R43] 按名字查找文件
来源：http://hz.guannengcc.top/gtqtxipyts.html

find . -name "*.log" -type f
来源：http://hz.guowangkeji.top/gtuheynhxe.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gtavixjdkq.html

find . -mtime -7 -type f
来源：http://hz.xuanzx.com/gtxptqdthn.html

[R45] 批量删除
来源：http://hz.hongshengwenyu.top/gtviaojzis.html

find . -name "*.tmp" -delete
来源：http://hz.guannengcc.top/gtksgznimy.html

[R46] 递归替换文件内容
来源：http://hz.bjfxy.top/gtqpzzaknv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.svipenyu.cn/gtemntlzxk.html

[R47] sed 单行替换
来源：http://hz.gotoacloud.top/gtpmvtbhpr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gotoacloud.top/gtvymgntyw.html

[R48] awk 取指定列
来源：http://hz.yuanzhike.top/gtqehaeddt.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtucihrmyw.html

[R49] awk 带条件
来源：http://hz.hysaishi.cn/gtqbcrvfdr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sxryk.cn/gtytmpjyii.html

[R50] awk 求和
来源：http://hz.xingfuxueyuan.xyz/gtrahrxkhq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cashguo.top/gtcoxilrwi.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gtdjscslwr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhengqikj.top/gtxhfdndkx.html

[R52] 统计行数
来源：http://hz.hongshengwenyu.top/gtnecutdnk.html

wc -l a.txt
来源：http://hz.hfpthk.cn/gtyazbrjsr.html

[R53] 查看文件头与实时尾
来源：http://hz.shuidangran.top/gtdeghxaub.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yanxiufei.cn/gtbzhjcbxh.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gtbrbfcqwk.html

diff a.txt b.txt
来源：http://hz.daxiang520.top/gttpsgnjlm.html

[R55] 压缩与解压
来源：http://hz.jinghuilouyu.cn/gtoqafbwsu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gtkijmwtfv.html

[R56] 远程拷贝
来源：http://hz.tianlin.xyz/gtywrnrjxg.html

scp file user@host:/path/
来源：http://hz.tianlin.xyz/gtubzadzed.html

[R57] 远程执行命令
来源：http://hz.yueranfly.top/gtkgofpila.html

ssh user@host 'uptime'
来源：http://hz.nwbrower.top/gtltghqxia.html

[R58] 下载文件
来源：http://hz.sysykeji.top/gtclpeztys.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenzaomai.com/gtcavknhgc.html

[R59] 发 POST JSON
来源：http://hz.quarkkingdee.top/gtnprjxbcx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtmknmrxml.html

[R60] 只看 HTTP 状态码
来源：http://hz.ppjwa.cn/gtdirdtcta.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zdqjudy.top/gtifqvzdgq.html

[R61] 磁盘占用
来源：http://hz.shzxlz.cn/gtmmelduzw.html

df -h;  du -sh *
来源：http://hz.sweek.top/gtxlukwxgy.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtkhztsnyx.html

du -ah . | sort -rh | head -10
来源：http://hz.cashguo.top/gthxuaqwlc.html

[R63] 内存与进程
来源：http://hz.0kj1m.cn/gthpcsnhkh.html

free -h;  ps aux | grep nginx
来源：http://hz.mhx1999.top/gtbsljztul.html

[R64] 结束进程
来源：http://hz.0kj1m.cn/gtguliqykm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xylfe.cn/gtyfrikwxj.html

[R65] 查看端口占用
来源：http://hz.zhongyouzk.top/gtinpryiie.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tianlin.xyz/gtwcbipkky.html

[R66] 定时任务
来源：http://hz.wangdashe.top/gtzvydrcga.html

crontab -e;  crontab -l
来源：http://hz.zhixingplan.top/gtdsjglpct.html

[R67] 生成随机十六进制串
来源：http://hz.hongshengwenyu.top/gtvnibgvpl.html

openssl rand -hex 16
来源：http://hz.xuetiantiany.cn/gtvupjfxaq.html

[R68] 计算文件校验值
来源：http://hz.ivvv.top/gtowydqkmi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hywenlv.cn/gtihveepkm.html

[R69] 生成随机密码
来源：http://hz.xuetiantiany.cn/gtgftwaxhj.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gthgfmscws.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtsuegxohp.html

date +%s;  date -d @1700000000
来源：http://hz.jinqigfzy.top/gtkzckjolk.html

[R71] 日期格式化
来源：http://hz.hnxiangtu.top/gtyviqttpa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.meibo888.top/gtmcezfxke.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gtodwmmswa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cashguo.top/gtmedbyume.html

[R73] 分割大日志
来源：http://hz.hysaishi.cn/gtmrrjalvq.html

split -l 1000 big.log part_
来源：http://hz.xuetiantiany.cn/gtsmkwlwfr.html

[R74] 批量重命名
来源：http://hz.shzxlz.cn/gttotmhhpo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yonumen.top/gtfbkmadti.html

[R75] 导出环境变量
来源：http://hz.316326.xyz/gtwgmpwbgv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tanke756.top/gtsngaxfqp.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtzybzofdj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtmjzgyqht.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtqloimoal.html

read -rp "请输入: " ans
来源：http://hz.guowangkeji.top/gtrwxylxvr.html

[R78] 交互式菜单
来源：http://hz.gaohongyu789.top/gtxwlskeds.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gtpiyyedtc.html

[R79] 解析命令行选项
来源：http://hz.chenlongwang.top/gtlvaejawi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gtzjkpphbh.html

[R80] 查看脚本执行耗时
来源：http://hz.9152youxi.cn/gtorsohjzi.html

time ./run.sh
来源：http://hz.vqdsnc.cn/gtjxqlsimd.html

================================================================================
来源：http://hz.cashguo.top/gtuczfagax.html

S. C / C++ 专题
来源：http://hz.xylfe.cn/gtcmtldffs.html

================================================================================
来源：http://hz.hammf.cn/gtxznjfgcu.html

[S01] C：Hello World
来源：http://hz.hfpthk.cn/gtxyzjawuv.html

#include <stdio.h>
来源：http://hz.xinyue.icu/gtlhpajmuq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zdqjudy.top/gttspjadfm.html

[S02] C：变量与格式化输出
来源：http://hz.ppjwa.cn/gtzcpolyrz.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgufenzy.top/gtlzwykisc.html

[S03] C：读入整数
来源：http://hz.xylfe.cn/gtnqxncxtx.html

int x; scanf("%d", &x);
来源：http://hz.hywenlv.cn/gtqdhqaeoy.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtmqkjudya.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnxiangtu.top/gtadoczdus.html

[S05] C：字符串长度
来源：http://hz.quarkkingdee.top/gttrayrsmn.html

strlen(s)
来源：http://hz.yuanzhike.top/gtdvqxcabs.html

[S06] C：字符串比较
来源：http://hz.wangshuangyany.cn/gtdxshywlf.html

strcmp(a, b) == 0
来源：http://hz.gaohongyu789.top/gttuidqylt.html

[S07] C：数组遍历求和
来源：http://hz.xziqi.cn/gtjhylqkck.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenzaomai.com/gtmutxedvf.html

[S08] C：动态内存分配与释放
来源：http://hz.ydzc1.top/gttqgeojws.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xylfe.cn/gtxvtndhvw.html

[S09] C：结构体定义与初始化
来源：http://hz.jinghuilouyu.cn/gtbkhpaxxs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.mhx1999.top/gtgwssyjwp.html

[S10] C：指针与解引用
来源：http://hz.tanke756.top/gtwnkyjboo.html

int *p = &a;  *p = 5;
来源：http://hz.cdnleiting.top/gtjnbpzbkf.html

[S11] C：逐行读文件
来源：http://hz.mhx1999.top/gtjzsxpmdv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.nanxuanxn.top/gtfxjbbkfc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gthvcbzybl.html

fclose(f);
来源：http://hz.iojbl.cn/gtvlcpktlf.html

[S12] C：写文件
来源：http://hz.chenjidiqi.icu/gthgryingt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cheryme.top/gtfpnpvzzk.html

[S13] C：宏定义
来源：http://hz.jinyuanbaomall.cn/gtjxswllpe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnxiangtu.top/gtlunzsnle.html

[S14] C：枚举
来源：http://hz.mhx1999.top/gtavsryurc.html


<!-- 参考信息 -->