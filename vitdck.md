代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.kuanghao11.cn/gtmgzasrlf.html

[Q52] 删除指定行
来源：http://hz.yj20258.top/gtrzhpbrjo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuxming.cn/gtmmudvgni.html

[Q53] 按条件删除
来源：http://hz.daria6918.cn/gtulsdzixc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guannengcc.top/gtqhuahxpr.html

[Q54] 清空表
来源：http://hz.guowangkeji.top/gtdfuqzbmj.html

TRUNCATE TABLE logs;
来源：http://hz.sweek.top/gtcighhanu.html

[Q55] 排名（并列占位）
来源：http://hz.zdqjudy.top/gtvkfmvabk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yanxiufei.cn/gtlwchrrfj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ywan-chungtsiang.top/gtfoknwuak.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sufxvd.cn/gtvlyjzqkj.html

[Q57] 行号
来源：http://hz.quarkkingdee.top/gtsmcblrbg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.316326.xyz/gtecfqllav.html

[Q58] 累计求和
来源：http://hz.jqgufenzy.top/gtsqcnxvwr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigfzy.top/gtliinbtnn.html

[Q59] 分组内累计
来源：http://hz.hnqzz.top/gtkuutfppx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtkgewwctz.html

[Q60] 取上一行 / 下一行
来源：http://hz.sweek.top/gtrcuygaes.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ywan-chungtsiang.top/gtgjypyrid.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daxiang520.top/gthpcnkqxv.html

[Q61] 移动平均
来源：http://hz.zhoulong.xyz/gtymbhsviv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aibaodan.cn/gtrubdchet.html

[Q62] 分组占比
来源：http://hz.aibaodan.cn/gthomiedwl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtxowqlfzj.html

[Q63] 开启事务
来源：http://hz.fengsongda.top/gtnohsdjvi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhiwuduotai.top/gthdlniexz.html

[Q64] 提交事务
来源：http://hz.zhoulong.xyz/gtoknynilf.html

COMMIT;
来源：http://hz.xuanzx.com/gtuhspvcpj.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtjunrghln.html

ROLLBACK;
来源：http://hz.zhiwuduotai.top/gtpcnnhxtr.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtiegxsbcg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ybcxt.top/gtbbbffemb.html

[Q67] 设置隔离级别
来源：http://hz.yuanzhike.top/gtykvidkzf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gtlfowscoh.html

[Q68] 保存点
来源：http://hz.guowangkeji.top/gtgafgqwzw.html

SAVEPOINT sp1;
来源：http://hz.cashguo.top/gtzcajbhct.html

ROLLBACK TO sp1;
来源：http://hz.jinghuilouyu.cn/gtgxeajiiy.html

[Q69] 查看执行计划
来源：http://hz.cqqwz.cn/gtlgwoknmv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yonumen.top/gtcgbjjmph.html

[Q70] 更新统计信息
来源：http://hz.tanke756.top/gtltorfchr.html

ANALYZE TABLE users;
来源：http://hz.gotoacloud.top/gtcyrgvqan.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtvzmcmtlr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fzhhl.top/gtiqiwdnzl.html

[Q72] 查看索引
来源：http://hz.cucudq.cn/gthkfjefsu.html

SHOW INDEX FROM users;
来源：http://hz.iojbl.cn/gtppbfgwcf.html

[Q73] 查看表状态
来源：http://hz.yonumen.top/gtkbdabbyy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zycfv.cn/gtmninqsmc.html

[Q74] 强制使用索引
来源：http://hz.tanke756.top/gtbrperrgj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.birdmap.top/gtbbrndalq.html

[Q75] 日期格式化
来源：http://hz.fzhhl.top/gtbtlirnuf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtcdefhrud.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtuawcsvqr.html

[Q76] 按天统计
来源：http://hz.daria6918.cn/gtzxuzcipl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuetiantiany.cn/gtsubvayqs.html

[Q77] 时间加减
来源：http://hz.yuanzhike.top/gthorxyxea.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuanzhike.top/gtxltokhbs.html

[Q78] 当前时间
来源：http://hz.zdqjudy.top/gthhmehkpa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangtech.top/gtfyxgejqq.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gtpzsjjcyx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guowangkeji.top/gtbdycwcbp.html

[Q80] 字符串截取
来源：http://hz.zhixingplan.top/gtvmacutqp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhengqikj.top/gtzfdjhino.html

[Q81] 字符串替换
来源：http://hz.cdnleiting.top/gtqbudsmma.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cucudq.cn/gtnxdcdogo.html

[Q82] 字符长度与字节长度
来源：http://hz.zhiwuduotai.top/gttbhomvdv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sweek.top/gtfvwihqqg.html

[Q83] 大小写转换
来源：http://hz.hysaishi.cn/gtkystqumt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gotoacloud.top/gtqiphiuni.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtixmedvcw.html

SELECT TRIM(name) FROM users;
来源：http://hz.wangdashe.top/gtkyreufmm.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtoqmvyfdx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hnqzz.top/gtbmwyomyd.html

[Q86] 读取 JSON 字段
来源：http://hz.ywan-chungtsiang.top/gttynmaaff.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtdjifmaad.html

[Q87] JSON 字段做条件
来源：http://hz.yanxiufei.cn/gticbpijpa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tian-w.cn/gtcdpnicny.html

[Q88] 行转列（条件聚合）
来源：http://hz.andypj.xyz/gtqdbpmvrx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ydzc1.top/gtviztfxup.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gtiscbakvf.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangtech.top/gtzanvhlsg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.wangshuangyany.cn/gtvxtfoagj.html

[Q90] 生成序号列
来源：http://hz.hfpthk.cn/gtsatozkaj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.bjfxy.top/gtroqicrhj.html

================================================================================
来源：http://hz.ivvv.top/gtuhvdztlp.html

R. Bash 专题
来源：http://hz.xuanzx.com/gtcwyentpd.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwsarhwoz.html

[R01] shebang 与严格模式
来源：http://hz.sysykeji.top/gtfnwioora.html

#!/usr/bin/env bash
来源：http://hz.tian-w.cn/gtangpusut.html

set -euo pipefail
来源：http://hz.chenzaomai.com/gthmunraye.html

[R02] 变量赋值与使用
来源：http://hz.smart0.xyz/gtbgywtjae.html

name="Tom"; echo "$name"
来源：http://hz.fengsongda.top/gthkrjzhju.html

[R03] 只读变量
来源：http://hz.0kj1m.cn/gtniqwhxaa.html

readonly PI=3.14
来源：http://hz.cheryme.top/gtdoykkddt.html

[R04] 位置参数
来源：http://hz.zdqjudy.top/gtiqgbsacr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.andypj.xyz/gtjyebjule.html

[R05] 参数默认值
来源：http://hz.jianghu66.top/gtbxzrbvdw.html

name="${1:-default}"
来源：http://hz.ybcxt.top/gtzyjtoing.html

[R06] 判断命令是否存在
来源：http://hz.fengsongda.top/gtstyiopcl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtaawmujro.html

[R07] if 判断文件
来源：http://hz.cheryme.top/gtawjsozyo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aizwys.cn/gtlbawmlhc.html

[R08] 数值比较
来源：http://hz.yonumen.top/gtuakeyijr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yangfankeji.com/gtjdwzpcpn.html

[R09] 字符串比较
来源：http://hz.tianlin.xyz/gtmjlvmlri.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.haohaochexian.top/gtdwmsehsn.html

[R10] 正则匹配
来源：http://hz.jqgfzy.top/gtqrhfxkci.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.c1oappe.top/gtsvkzqvtq.html

[R11] case 多分支
来源：http://hz.jiagoushi.top/gtkcdlzbse.html

case "$1" in
来源：http://hz.havefunace.top/gtqpoglirx.html

start) echo "启动" ;;
来源：http://hz.shangyingyoupin.top/gtsxvxnjub.html

stop)  echo "停止" ;;
来源：http://hz.cucudq.cn/gtgucuntue.html

*)     echo "未知命令" ;;
来源：http://hz.gogol.net.cn/gtlktpmwrh.html

esac
来源：http://hz.jinqigufen.top/gtsqaesuew.html

[R12] for 遍历文件
来源：http://hz.xuetiantiany.cn/gtbkcmeeia.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cucudq.cn/gthgjjhxhx.html

[R13] for 计数循环
来源：http://hz.jinqigfzy.top/gttevvpmrw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sufxvd.cn/gtlckkkhzv.html

[R14] C 风格 for
来源：http://hz.cucudq.cn/gtjqiesady.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sufxvd.cn/gtxeidkeqy.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gtupwqaxbm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dashuyun.cn/gtorgyeerj.html

[R16] until 等待条件
来源：http://hz.vqdsnc.cn/gtyqcbwano.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhixingplan.top/gtugoziqmm.html

[R17] 数组定义与取值
来源：http://hz.aibaodan.cn/gtebpcmuua.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nwbrower.top/gtgjlomsbw.html

[R18] 遍历数组
来源：http://hz.snrcjt.cn/gtzexrygyq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yvedp.cn/gtsnomnuwz.html

[R19] 数组长度
来源：http://hz.aibaodan.cn/gtunlhxmso.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtvdvjjmnk.html

[R20] 关联数组（字典）
来源：http://hz.zhengqikj.top/gtpttgjgzx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.bjfxy.top/gtziywotth.html

[R21] 字符串长度
来源：http://hz.hnxiangtu.top/gtkpihtylv.html

echo "${#s}"
来源：http://hz.ivvv.top/gtqvpokmqi.html

[R22] 截取子串
来源：http://hz.daxiang520.top/gtljivqrza.html

echo "${s:0:5}"
来源：http://hz.smart0.xyz/gtkmahbsat.html

[R23] 字符串替换
来源：http://hz.hnqzz.top/gtetevzpby.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtegiazwdo.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtnohpiqvi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.9152youxi.cn/gtvawkikee.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtxkuovduo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sufxvd.cn/gtivpfitgk.html

[R26] 命令替换
来源：http://hz.yj20258.top/gtvlvrvemp.html

now=$(date +%F); echo "$now"
来源：http://hz.fengsongda.top/gtwdncjdqt.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtomqyoxgw.html

echo $((1 + 2 * 3))
来源：http://hz.gaohongyu789.top/gtyrsagjrj.html

[R28] 浮点运算
来源：http://hz.zhoulong.xyz/gtlwldxojk.html

echo "scale=2; 10/3" | bc
来源：http://hz.meibo888.top/gtzlngdrab.html

[R29] 定义函数
来源：http://hz.snrcjt.cn/gteldocdnq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj202588.top/gtnawrnvka.html

[R30] 函数返回状态码
来源：http://hz.pycfn.com/gttuhfucja.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtwsrdowdk.html

[R31] 局部变量
来源：http://hz.yangfankeji.com/gtigkpsvsv.html

f() { local x=1; echo "$x"; }
来源：http://hz.xylfe.cn/gtlzzywdaj.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gttssicikb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.316326.xyz/gtdlrotypp.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gtfvbspqbn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ivvv.top/gtnxpxhntr.html

[R34] 退出时清理
来源：http://hz.haohaochexian.top/gtwpgpeghk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtmkyrtrwm.html

[R35] 后台执行并等待
来源：http://hz.gzhubu.top/gtlrzzuqlc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.snrcjt.cn/gtfzapxtkx.html

[R36] 并发执行多个任务
来源：http://hz.xinyue.icu/gtnzoprwwp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jiagoushi.top/gthjhnyvjr.html

[R37] 把输出赋给变量
来源：http://hz.pycfn.com/gtfcvjwvru.html

files=$(ls -1)
来源：http://hz.jyoumei.cn/gtjccypfby.html

[R38] 管道串联
来源：http://hz.guowangkeji.top/gtujxnghzr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yvedp.cn/gtgjowxgcw.html

[R39] 重定向标准输出与错误
来源：http://hz.zhongyouzk.top/gtchjygmon.html

cmd > out.log 2>&1
来源：http://hz.andypj.xyz/gtahndrbaz.html

[R40] 追加写日志
来源：http://hz.jlsjyb.cn/gtwzeijkvl.html

echo "log" >> out.log
来源：http://hz.smart0.xyz/gtpesofkmp.html

[R41] 丢弃输出
来源：http://hz.yuanzhike.top/gtopkmcibv.html

cmd >/dev/null 2>&1
来源：http://hz.ivvv.top/gtexozpmow.html

[R42] 输入重定向
来源：http://hz.hysaishi.cn/gtydgxqrhk.html

wc -l < a.txt
来源：http://hz.ywan-chungtsiang.top/gtwememopv.html

[R43] 按名字查找文件
来源：http://hz.zhengqikj.top/gtazskjvwz.html

find . -name "*.log" -type f
来源：http://hz.sufxvd.cn/gtflvzqskd.html

[R44] 按修改时间查找
来源：http://hz.gzhubu.top/gtcidcyizs.html

find . -mtime -7 -type f
来源：http://hz.hnxiangtu.top/gtupitcmty.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtovpsjpxf.html

find . -name "*.tmp" -delete
来源：http://hz.nanxuanxn.top/gtxbhywdsq.html

[R46] 递归替换文件内容
来源：http://hz.cheryme.top/gtpbtowjgs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guannengcc.top/gtxjaxmkaf.html

[R47] sed 单行替换
来源：http://hz.guannengcc.top/gtpcocqunb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.316326.xyz/gtijddqlip.html

[R48] awk 取指定列
来源：http://hz.shangyingyoupin.top/gthwjnwgyt.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj202588.top/gtzpyeubkn.html

[R49] awk 带条件
来源：http://hz.yuxming.cn/gttmlrevil.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenzaomai.com/gtjfskhuzc.html

[R50] awk 求和
来源：http://hz.shzxlz.cn/gtjckizzph.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigufen.top/gtakhpxznf.html

[R51] 排序去重取前几
来源：http://hz.zhengqikj.top/gtoeulmzij.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xingfuxueyuan.xyz/gttrfzjgji.html

[R52] 统计行数
来源：http://hz.yangfankeji.com/gtfpqzdfxu.html

wc -l a.txt
来源：http://hz.hywenlv.cn/gtotbitwuf.html

[R53] 查看文件头与实时尾
来源：http://hz.pengpengdd.cyou/gtkuwdbaji.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtwwmzyzxj.html

[R54] 比较两个文件
来源：http://hz.ppjwa.cn/gtfbouvskl.html

diff a.txt b.txt
来源：http://hz.jinyuanbaomall.cn/gtingubgwi.html

[R55] 压缩与解压
来源：http://hz.dianchejie.cn/gtcytfzlce.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhongyouzk.top/gtobjgnqxs.html

[R56] 远程拷贝
来源：http://hz.zdqjudy.top/gtcprwtpfx.html

scp file user@host:/path/
来源：http://hz.nwbrower.top/gtwvgjqzmz.html

[R57] 远程执行命令
来源：http://hz.yj202588.top/gtrjvfeelu.html

ssh user@host 'uptime'
来源：http://hz.xziqi.cn/gtbyceewun.html

[R58] 下载文件
来源：http://hz.zycfv.cn/gtfvivyvme.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.snrcjt.cn/gtcmmyimph.html

[R59] 发 POST JSON
来源：http://hz.xinyue.icu/gtwjpwgcly.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.316326.xyz/gtxvqguopy.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtdhiiofji.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtqxilcmqi.html

[R61] 磁盘占用
来源：http://hz.hnxiangtu.top/gtqefqurqt.html

df -h;  du -sh *
来源：http://hz.hfpthk.cn/gtepfozzfx.html

[R62] 找最占空间的文件
来源：http://hz.pengpengdd.cyou/gtrhfqdeui.html

du -ah . | sort -rh | head -10
来源：http://hz.chenjidiqi.icu/gtbwaorpse.html

[R63] 内存与进程
来源：http://hz.jlsjyb.cn/gtfdmjmnfn.html

free -h;  ps aux | grep nginx
来源：http://hz.sysykeji.top/gtlbxuplgt.html

[R64] 结束进程
来源：http://hz.kuanghao11.cn/gtxesqwseo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gtirkjdgry.html

[R65] 查看端口占用
来源：http://hz.daria6918.cn/gtyabbsypo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj202588.top/gttcdfvdms.html

[R66] 定时任务
来源：http://hz.cqqwz.cn/gtsjpkglgg.html

crontab -e;  crontab -l
来源：http://hz.c1oappe.top/gtpycaduua.html

[R67] 生成随机十六进制串
来源：http://hz.pycfn.com/gtukyhjzsr.html

openssl rand -hex 16
来源：http://hz.iojbl.cn/gtwxrliiix.html

[R68] 计算文件校验值
来源：http://hz.gotoacloud.top/gtqggvxyvo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtliaradxq.html

[R69] 生成随机密码
来源：http://hz.hnxiangtu.top/gtfqpyhmdb.html

head -c 16 /dev/urandom | base64
来源：http://hz.yonumen.top/gtclrqbjwt.html

[R70] 时间戳与互转
来源：http://hz.ivvv.top/gtukmxziau.html

date +%s;  date -d @1700000000
来源：http://hz.andypj.xyz/gtcxlxixoa.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gtcdrwrrah.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tian-w.cn/gtycnciejd.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gtvyahvhmp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xylfe.cn/gtgmgoxfjv.html

[R73] 分割大日志
来源：http://hz.xinyue.icu/gtdkjrjgza.html

split -l 1000 big.log part_
来源：http://hz.sxryk.cn/gtxqqflmlt.html

[R74] 批量重命名
来源：http://hz.tian-w.cn/gthnwmwdik.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtfliarzog.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtvcjzxxod.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.feifeiyinyue.top/gterhlipmu.html

[R76] 使用临时文件
来源：http://hz.hfpthk.cn/gtwsiklsbr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtldhupeqq.html

[R77] 读取用户输入
来源：http://hz.yonumen.top/gtclrjbjym.html

read -rp "请输入: " ans
来源：http://hz.aibaodan.cn/gtgfhwmhvm.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtmxuoyvcc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhoulong.xyz/gtxjbqjnjs.html

[R79] 解析命令行选项
来源：http://hz.zhengqikj.top/gtolmgmmls.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gtcphqrtat.html

[R80] 查看脚本执行耗时
来源：http://hz.hysaishi.cn/gtbchvdnmh.html

time ./run.sh
来源：http://hz.iojbl.cn/gtkodrytuv.html

================================================================================
来源：http://hz.sufxvd.cn/gtgqxghlfr.html

S. C / C++ 专题
来源：http://hz.hnxiangtu.top/gtmmrrppqt.html

================================================================================
来源：http://hz.birdmap.top/gtaofjezbq.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtzwxyhgkd.html

#include <stdio.h>
来源：http://hz.jianghu66.top/gtbtgxkdop.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenjidiqi.icu/gttkbakhxl.html

[S02] C：变量与格式化输出
来源：http://hz.xinyue.icu/gttlcavgsm.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtogxbligr.html

[S03] C：读入整数
来源：http://hz.yongpay.top/gtdkhsefsf.html

int x; scanf("%d", &x);
来源：http://hz.fengsongda.top/gttkdyepee.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtsqalpcuv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgufenzy.top/gtjncbipid.html

[S05] C：字符串长度
来源：http://hz.havefunace.top/gtajoqhxnt.html

strlen(s)
来源：http://hz.cheryme.top/gtdwvkcnmg.html

[S06] C：字符串比较
来源：http://hz.hysaishi.cn/gtfatsmzdu.html

strcmp(a, b) == 0
来源：http://hz.jianghu66.top/gtpekibdfa.html

[S07] C：数组遍历求和
来源：http://hz.quarkkingdee.top/gtnughqehn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgfzy.top/gthaipjzjv.html

[S08] C：动态内存分配与释放
来源：http://hz.gzhubu.top/gtcuwzfvon.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtssgkjpbi.html

[S09] C：结构体定义与初始化
来源：http://hz.jinyuanbaomall.cn/gtbsotbavq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guowangkeji.top/gtzmvtwami.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtagmevwgc.html

int *p = &a;  *p = 5;
来源：http://hz.hnxiangtu.top/gttmcjyonn.html

[S11] C：逐行读文件
来源：http://hz.quarkkingdee.top/gtlxwsaksb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.feifeiyinyue.top/gtqwyqdmhn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tanke756.top/gtlroerddq.html

fclose(f);
来源：http://hz.xylfe.cn/gthwhyzhei.html

[S12] C：写文件
来源：http://hz.zhengqikj.top/gtpbhvprbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ywan-chungtsiang.top/gtmbsxmjaw.html

[S13] C：宏定义
来源：http://hz.andypj.xyz/gtwaxaurxx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dianchejie.cn/gtfgccrzak.html

[S14] C：枚举
来源：http://hz.xuetiantiany.cn/gtxczpaujk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.feifeiyinyue.top/gtmiwagxyc.html

[S15] C：类型转换
来源：http://hz.tianlin.xyz/gtgmaaazhu.html

(double) a / b
来源：http://hz.yj20258888.top/gteugvzhgs.html

[S16] C：位操作置位
来源：http://hz.zhoulong.xyz/gtptvekltb.html

x |= (1 << 3);
来源：http://hz.sxryk.cn/gtazrtznry.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtlgceofrr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.c1oappe.top/gtznehxekg.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangtech.top/gtwzsfhgpx.html

int main(int argc, char **argv)
来源：http://hz.chenlongwang.top/gtnvcqjrke.html

[S19] C：快速排序
来源：http://hz.yvedp.cn/gtuolpikfv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gtdouvclbx.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtceehhydc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtsgrgrtbt.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gtxrgkpghi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangshuangyany.cn/gteoopazak.html

[S22] C：字符串转数字
来源：http://hz.jqgfzy.top/gtesnejepq.html


<!-- 参考信息 -->