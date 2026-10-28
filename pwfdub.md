代发 wailian999

[Q63] 开启事务
来源：http://hz.andypj.xyz/gthcgpvouc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangdashe.top/gtoludxjxl.html

[Q64] 提交事务
来源：http://hz.jinqigfzy.top/gtygygyamc.html

COMMIT;
来源：http://hz.jlsjyb.cn/gtcjkqqagk.html

[Q65] 回滚事务
来源：http://hz.pengpengdd.cyou/gtzbdqszik.html

ROLLBACK;
来源：http://hz.ywan-chungtsiang.top/gthekyuuhb.html

[Q66] 行锁查询
来源：http://hz.cashguo.top/gtvgfxwrva.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtzdtvxpjw.html

[Q67] 设置隔离级别
来源：http://hz.zhaomingkeji.xyz/gtlgjmlbvj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnxiangtu.top/gttgruocqj.html

[Q68] 保存点
来源：http://hz.ehwqpu.com/gtdoyjyajn.html

SAVEPOINT sp1;
来源：http://hz.hnxiangtu.top/gtrdpneivq.html

ROLLBACK TO sp1;
来源：http://hz.nanxinkj.top/gthlcjkggs.html

[Q69] 查看执行计划
来源：http://hz.sysykeji.top/gthraabmgc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenzaomai.com/gtedtpfgfr.html

[Q70] 更新统计信息
来源：http://hz.xuanzx.com/gtzeaibvgx.html

ANALYZE TABLE users;
来源：http://hz.52xcode.cn/gtsdhaspwy.html

[Q71] 查看建表语句
来源：http://hz.zhiwuduotai.top/gtogorynbi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ppjwa.cn/gtiyvhxnrg.html

[Q72] 查看索引
来源：http://hz.sweek.top/gtiwklffum.html

SHOW INDEX FROM users;
来源：http://hz.yj20258.top/gtdphoyolh.html

[Q73] 查看表状态
来源：http://hz.chenlongwang.top/gtbuaupoum.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hywenlv.cn/gtzsgvahmh.html

[Q74] 强制使用索引
来源：http://hz.sweek.top/gtrlumoeqr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtldhjlrna.html

[Q75] 日期格式化
来源：http://hz.jinqigufen.top/gtadxmppdy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtucyjdkqe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dianchejie.cn/gtswyuijyu.html

[Q76] 按天统计
来源：http://hz.c1oappe.top/gtgzxohryx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtqcyahhkr.html

[Q77] 时间加减
来源：http://hz.hnxiangtu.top/gtocwnlabg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinyuanbaomall.cn/gtynkjmyod.html

[Q78] 当前时间
来源：http://hz.aizwys.cn/gtnlewztwp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hysaishi.cn/gtcfxspjap.html

[Q79] 字符串拼接
来源：http://hz.zhaomingkeji.xyz/gtjfhroutd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gtxiauzqlf.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtvvxyggny.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.birdmap.top/gtznulfjaa.html

[Q81] 字符串替换
来源：http://hz.cucudq.cn/gtwriwbeot.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhoulong.xyz/gtfqokstrm.html

[Q82] 字符长度与字节长度
来源：http://hz.zhixingplan.top/gtzebuplah.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtzgpieqyv.html

[Q83] 大小写转换
来源：http://hz.zdqjudy.top/gtxoedtfjs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.mhx1999.top/gtysxytvzs.html

[Q84] 去除首尾空格
来源：http://hz.jiagoushi.top/gtldxcizdg.html

SELECT TRIM(name) FROM users;
来源：http://hz.cheryme.top/gtgcgselkl.html

[Q85] 数值取整
来源：http://hz.gotoacloud.top/gtsdrhqose.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jlsjyb.cn/gttovxpvrk.html

[Q86] 读取 JSON 字段
来源：http://hz.zhongyouzk.top/gtwaxgswec.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aizwys.cn/gtdocbvskd.html

[Q87] JSON 字段做条件
来源：http://hz.yanxiufei.cn/gtnxwxtqwr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zdqjudy.top/gtoktkntru.html

[Q88] 行转列（条件聚合）
来源：http://hz.jianghu66.top/gthszqxazk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangshuangyany.cn/gtgqpchdlj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hysaishi.cn/gtuhnudjcn.html

[Q89] 判断表是否存在
来源：http://hz.snrcjt.cn/gtcbemyvez.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daxiang520.top/gtcsphdbek.html

[Q90] 生成序号列
来源：http://hz.aibaodan.cn/gtmjrggefc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zdqjudy.top/gtkpmojsid.html

================================================================================
来源：http://hz.havefunace.top/gtinwwqbbx.html

R. Bash 专题
来源：http://hz.ybcxt.top/gtvkownrsi.html

================================================================================
来源：http://hz.jqgfzy.top/gtsvomaxsn.html

[R01] shebang 与严格模式
来源：http://hz.cqqwz.cn/gtiajqsory.html

#!/usr/bin/env bash
来源：http://hz.zhaomingkeji.xyz/gtqzajnbja.html

set -euo pipefail
来源：http://hz.zdqjudy.top/gtrsxpryrb.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gtniwpukvm.html

name="Tom"; echo "$name"
来源：http://hz.yuxming.cn/gtdznxgeim.html

[R03] 只读变量
来源：http://hz.gogol.net.cn/gtkecnzith.html

readonly PI=3.14
来源：http://hz.shangyingyoupin.top/gtypxegvpq.html

[R04] 位置参数
来源：http://hz.xuetiantiany.cn/gtmecrjowq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gtpboqgxdz.html

[R05] 参数默认值
来源：http://hz.kuanghao11.cn/gtxuzfwfhk.html

name="${1:-default}"
来源：http://hz.guannengcc.top/gtegerghup.html

[R06] 判断命令是否存在
来源：http://hz.pengpengdd.cyou/gtmeobmslk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnqzz.top/gtyozuxqzj.html

[R07] if 判断文件
来源：http://hz.ybcxt.top/gtikasfvgj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hfpthk.cn/gtswwdhrog.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gthxykcmcu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangtech.top/gtnwlocadj.html

[R09] 字符串比较
来源：http://hz.hongshengwenyu.top/gtctetitpb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.chenlongwang.top/gtnrmqwtso.html

[R10] 正则匹配
来源：http://hz.ivvv.top/gtaadgpthi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.wangdashe.top/gttwlnudqt.html

[R11] case 多分支
来源：http://hz.jinyuanbaomall.cn/gtjowjkxzr.html

case "$1" in
来源：http://hz.yvedp.cn/gtkpayvnsm.html

start) echo "启动" ;;
来源：http://hz.316326.xyz/gtaqckvjyp.html

stop)  echo "停止" ;;
来源：http://hz.guowangkeji.top/gthzmpyjty.html

*)     echo "未知命令" ;;
来源：http://hz.yanxiufei.cn/gtkbnfpuxn.html

esac
来源：http://hz.daxiang520.top/gtcqzpkacl.html

[R12] for 遍历文件
来源：http://hz.jinghuilouyu.cn/gtwbssnxob.html

for f in *.txt; do echo "$f"; done
来源：http://hz.havefunace.top/gtpxhebwln.html

[R13] for 计数循环
来源：http://hz.hnxiangtu.top/gtzmqzseeq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sufxvd.cn/gtuwqhjytn.html

[R14] C 风格 for
来源：http://hz.yj20258888.top/gtuaucutti.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtdceqielw.html

[R15] while 逐行读文件
来源：http://hz.vqdsnc.cn/gtycqabcap.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shanyushiyangkeji.top/gtgttylckp.html

[R16] until 等待条件
来源：http://hz.yvedp.cn/gtkjtthqff.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jqgufenzy.top/gtibzmmooj.html

[R17] 数组定义与取值
来源：http://hz.0kj1m.cn/gthzbnlxsc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sweek.top/gtbwfinjow.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtdmxnzfbn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtydeqrcpz.html

[R19] 数组长度
来源：http://hz.shanyushiyangkeji.top/gtjvkgsawq.html

echo "${#arr[@]}"
来源：http://hz.zhijiandao.cn/gtvadmsrsz.html

[R20] 关联数组（字典）
来源：http://hz.ydzc1.top/gtkkgpaaot.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.snrcjt.cn/gtltkfjmim.html

[R21] 字符串长度
来源：http://hz.xziqi.cn/gtckoduzbx.html

echo "${#s}"
来源：http://hz.snrcjt.cn/gtynuhdawk.html

[R22] 截取子串
来源：http://hz.52xcode.cn/gtalcmbowl.html

echo "${s:0:5}"
来源：http://hz.jinqigfzy.top/gtlgwjhifq.html

[R23] 字符串替换
来源：http://hz.havefunace.top/gtrxcwskti.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhijiandao.cn/gtjxdrlkcp.html

[R24] 大小写转换
来源：http://hz.gogol.net.cn/gtfszhzwvw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gaohongyu789.top/gtybctiqoy.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhijiandao.cn/gtiwegnttc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangdashe.top/gtqeprayim.html

[R26] 命令替换
来源：http://hz.aizwys.cn/gtmgswufxv.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigufen.top/gtsgzbutxw.html

[R27] 算术展开
来源：http://hz.jinqigfzy.top/gtpsgcsjpk.html

echo $((1 + 2 * 3))
来源：http://hz.hnqzz.top/gtyhvrkcqe.html

[R28] 浮点运算
来源：http://hz.jianghu66.top/gtrqifazcq.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenjidiqi.icu/gtxetjrinv.html

[R29] 定义函数
来源：http://hz.kuanghao11.cn/gtwvpscmir.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.kuanghao11.cn/gtorvawkio.html

[R30] 函数返回状态码
来源：http://hz.meibo888.top/gtnxcmrcvo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtkpynvvak.html

[R31] 局部变量
来源：http://hz.ivvv.top/gtrxrkxavh.html

f() { local x=1; echo "$x"; }
来源：http://hz.vqdsnc.cn/gtsfvnbchm.html

[R32] 参数个数校验
来源：http://hz.yuxming.cn/gtrxaoqkhi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.smart0.xyz/gtclebezoo.html

[R33] 捕获错误并提示行号
来源：http://hz.guowangkeji.top/gttnxvjnco.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhongyouzk.top/gtgmvprxih.html

[R34] 退出时清理
来源：http://hz.zhengqikj.top/gtitmampip.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gtzroblzgl.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gtrolydvpx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gogol.net.cn/gtunrzxfcl.html

[R36] 并发执行多个任务
来源：http://hz.316326.xyz/gtcupimfls.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xuanzx.com/gtfnnoxmux.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtoebpcizd.html

files=$(ls -1)
来源：http://hz.jinyuanbaomall.cn/gtwpooykqr.html

[R38] 管道串联
来源：http://hz.kuanghao11.cn/gtistmdcyt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gogol.net.cn/gtevqbhsky.html

[R39] 重定向标准输出与错误
来源：http://hz.yuanzhike.top/gtcmoiisja.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtiduzdvfy.html

[R40] 追加写日志
来源：http://hz.zhengqikj.top/gtgqkouzkd.html

echo "log" >> out.log
来源：http://hz.jinyuanbaomall.cn/gttxptlhbs.html

[R41] 丢弃输出
来源：http://hz.kuanghao11.cn/gthimacnbp.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtyolufrnj.html

[R42] 输入重定向
来源：http://hz.jianghu66.top/gthbxmnswm.html

wc -l < a.txt
来源：http://hz.sysykeji.top/gtggndbyms.html

[R43] 按名字查找文件
来源：http://hz.yj202588.top/gtzrateocb.html

find . -name "*.log" -type f
来源：http://hz.hfpthk.cn/gtlaymjbnt.html

[R44] 按修改时间查找
来源：http://hz.chenjidiqi.icu/gtoygxyvpj.html

find . -mtime -7 -type f
来源：http://hz.guowangkeji.top/gtfjthaixn.html

[R45] 批量删除
来源：http://hz.nanxinkj.top/gtnmxrgavk.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtlrlbnkca.html

[R46] 递归替换文件内容
来源：http://hz.ydjk.org.cn/gtyiluaedk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hywenlv.cn/gtjaiqeerb.html

[R47] sed 单行替换
来源：http://hz.chenlongwang.top/gtrlxukzgs.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhoulong.xyz/gtamfvuebp.html

[R48] awk 取指定列
来源：http://hz.xuetiantiany.cn/gtwbrmypwy.html

awk '{print $1, $3}' a.txt
来源：http://hz.nwbrower.top/gtiahpamqj.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtthyzdidg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cheryme.top/gtvjjotwdk.html

[R50] awk 求和
来源：http://hz.yj202588.top/gtjruvlija.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhengqikj.top/gtlwzgbinl.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtkqlenznb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.havefunace.top/gtdxjpxvql.html

[R52] 统计行数
来源：http://hz.chenzaomai.com/gtcavgagrg.html

wc -l a.txt
来源：http://hz.yj20258.top/gtkcymmbfv.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtjhgrtjet.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tianlin.xyz/gtgrepvynm.html

[R54] 比较两个文件
来源：http://hz.nwbrower.top/gtozqmajbi.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gtlfbnnyjz.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtvxhvsatw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.smart0.xyz/gtttwyozmt.html

[R56] 远程拷贝
来源：http://hz.hongshengwenyu.top/gtowyslvjf.html

scp file user@host:/path/
来源：http://hz.jlsjyb.cn/gtfwykvdoe.html

[R57] 远程执行命令
来源：http://hz.jiagoushi.top/gtogxqbvfr.html

ssh user@host 'uptime'
来源：http://hz.bjfxy.top/gtburcfqvw.html

[R58] 下载文件
来源：http://hz.hysaishi.cn/gtxnlssoxi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenjidiqi.icu/gticdtijaq.html

[R59] 发 POST JSON
来源：http://hz.dianchejie.cn/gtfolijaqr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtfmqlmlsg.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtcrksrfut.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangshuangyany.cn/gtrzzswwny.html

[R61] 磁盘占用
来源：http://hz.feifeiyinyue.top/gtryvnescw.html

df -h;  du -sh *
来源：http://hz.jinqigufen.top/gtgvknylml.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gtqjuhojvw.html

du -ah . | sort -rh | head -10
来源：http://hz.gogol.net.cn/gtrlpudfoz.html

[R63] 内存与进程
来源：http://hz.hysaishi.cn/gtzyrqsuhq.html

free -h;  ps aux | grep nginx
来源：http://hz.fengsongda.top/gtkfghitke.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtcsxmgfdo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jianghu66.top/gtscebadrx.html

[R65] 查看端口占用
来源：http://hz.xylfe.cn/gtngikzraj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtnjwslnqp.html

[R66] 定时任务
来源：http://hz.zycfv.cn/gtbpbvhgvc.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtcuwtzlaj.html

[R67] 生成随机十六进制串
来源：http://hz.zdqjudy.top/gtrpsirpry.html

openssl rand -hex 16
来源：http://hz.chenzaomai.com/gtcnxoitui.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gthycqquud.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dashuyun.cn/gtkfxxuclr.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtuwlupuah.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxuanxn.top/gtbzegebjr.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangtech.top/gtczvttkdw.html

date +%s;  date -d @1700000000
来源：http://hz.svipenyu.cn/gthjcbgdjp.html

[R71] 日期格式化
来源：http://hz.yj20258888.top/gtwljnpcfi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhaomingkeji.xyz/gtwskgjuet.html

[R72] 等待端口就绪
来源：http://hz.aibaodan.cn/gtkahbpfda.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.fzhhl.top/gtnheddclw.html

[R73] 分割大日志
来源：http://hz.tanke756.top/gtqwblwaqg.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtiophwgxh.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtwxickqzt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxuanxn.top/gtszaysclk.html

[R75] 导出环境变量
来源：http://hz.hammf.cn/gtfrelxmpq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jyoumei.cn/gttrusalsk.html

[R76] 使用临时文件
来源：http://hz.sxryk.cn/gtigrcwxod.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtjqeowung.html

[R77] 读取用户输入
来源：http://hz.cheryme.top/gtyxvxdvdi.html

read -rp "请输入: " ans
来源：http://hz.gaohongyu789.top/gtdpcfrqrx.html

[R78] 交互式菜单
来源：http://hz.jlsjyb.cn/gtkltdfldw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dashuyun.cn/gtsrnimmib.html

[R79] 解析命令行选项
来源：http://hz.birdmap.top/gtnwcvesrg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gtwkpejjox.html

[R80] 查看脚本执行耗时
来源：http://hz.tanke756.top/gtslkmesit.html

time ./run.sh
来源：http://hz.gaohongyu789.top/gteviliaim.html

================================================================================
来源：http://hz.fzhhl.top/gtmpdzjwju.html

S. C / C++ 专题
来源：http://hz.gzhubu.top/gtbbfrexjm.html

================================================================================
来源：http://hz.quarkkingdee.top/gtlckfktzx.html

[S01] C：Hello World
来源：http://hz.nwbrower.top/gtowdsmlib.html

#include <stdio.h>
来源：http://hz.shanyushiyangtech.top/gtxgprvvfg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.316326.xyz/gtotsyiaye.html

[S02] C：变量与格式化输出
来源：http://hz.yuanzhike.top/gtkqjlermz.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuanzhike.top/gturvmdkjd.html

[S03] C：读入整数
来源：http://hz.xuetiantiany.cn/gttrrjgsjw.html

int x; scanf("%d", &x);
来源：http://hz.bjfxy.top/gtylofwqeh.html

[S04] C：字符串复制
来源：http://hz.tian-w.cn/gtkhgmbphm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtjhcuyver.html

[S05] C：字符串长度
来源：http://hz.svipenyu.cn/gtfkxnlhqw.html

strlen(s)
来源：http://hz.quarkkingdee.top/gtdjiyhrov.html

[S06] C：字符串比较
来源：http://hz.jianghu66.top/gtbnvhpxel.html

strcmp(a, b) == 0
来源：http://hz.andypj.xyz/gtnwdabvjh.html

[S07] C：数组遍历求和
来源：http://hz.jiagoushi.top/gtqwuiyudj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daxiang520.top/gtcrbkpeoa.html

[S08] C：动态内存分配与释放
来源：http://hz.aibaodan.cn/gtwubvgkgx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuetiantiany.cn/gthtutleyh.html

[S09] C：结构体定义与初始化
来源：http://hz.sufxvd.cn/gtzncgebnw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sweek.top/gtgdgmvzli.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtkwqpmxir.html

int *p = &a;  *p = 5;
来源：http://hz.yongpay.top/gtxhsmbdwe.html

[S11] C：逐行读文件
来源：http://hz.guannengcc.top/gtwrgqsmah.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jyoumei.cn/gtwjamnfgu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pengpengdd.cyou/gtkmfdwpnb.html

fclose(f);
来源：http://hz.daria6918.cn/gtronaebvx.html

[S12] C：写文件
来源：http://hz.pengpengdd.cyou/gtmtkzzfyh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jqgufenzy.top/gtpmfykfpt.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtbmzdifrz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtzfyifxyp.html

[S14] C：枚举
来源：http://hz.xylfe.cn/gttsejihpz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shanyushiyangkeji.top/gteqtiygrr.html

[S15] C：类型转换
来源：http://hz.xylfe.cn/gtkknjypcs.html

(double) a / b
来源：http://hz.xuetiantiany.cn/gtnelgpypd.html

[S16] C：位操作置位
来源：http://hz.havefunace.top/gtrtnikwkf.html

x |= (1 << 3);
来源：http://hz.smart0.xyz/gtafbnzdjc.html

[S17] C：安全拼接字符串
来源：http://hz.jqgufenzy.top/gtjvedmcyu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cashguo.top/gtjfnwmdvw.html

[S18] C：命令行参数
来源：http://hz.yvedp.cn/gtluoswxeu.html

int main(int argc, char **argv)
来源：http://hz.xingfuxueyuan.xyz/gtkduhqbzc.html

[S19] C：快速排序
来源：http://hz.cucudq.cn/gtvqkodjja.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gotoacloud.top/gtsbaqyhlw.html

[S20] C：二分查找
来源：http://hz.quarkkingdee.top/gtetuokobr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtjtafkkiz.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtmggezrqn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigfzy.top/gtoqlewqit.html

[S22] C：字符串转数字
来源：http://hz.52xcode.cn/gtxnlyuhtg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ybcxt.top/gtsnzowvml.html

[S23] C：随机数
来源：http://hz.sufxvd.cn/gtayjekjkb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtxthxuazy.html

[S24] C：获取本地时间
来源：http://hz.dashuyun.cn/gtqneddupb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gtbzgaqgzl.html

[S25] C：内存拷贝
来源：http://hz.sufxvd.cn/gtembgglhp.html

memcpy(dst, src, n);
来源：http://hz.chenlongwang.top/gtithzynsg.html

[S26] C：内存清零
来源：http://hz.smart0.xyz/gtrusxcymd.html

memset(a, 0, sizeof a);
来源：http://hz.shzxlz.cn/gtwvwjjwms.html

[S27] C：定义常量
来源：http://hz.zdqjudy.top/gtreeivzna.html

const double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtnijwyhod.html

[S28] C：静态变量
来源：http://hz.jyoumei.cn/gtrfilewpe.html

static int counter = 0;
来源：http://hz.tian-w.cn/gtejgmihyl.html

[S29] C：变参函数
来源：http://hz.sxryk.cn/gtmqagwgwq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sweek.top/gtswfwoqur.html

[S30] C：头文件保护
来源：http://hz.yueranfly.top/gtcofvbfhk.html

#ifndef X_H
来源：http://hz.chenlongwang.top/gtbvpuvboo.html

#define X_H
来源：http://hz.dianchejie.cn/gtwycamxle.html

#endif
来源：http://hz.xziqi.cn/gtbeuxingg.html

[S31] C++：Hello World
来源：http://hz.xziqi.cn/gtvnzhpzim.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtitnvboqb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gtuapqgnso.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtdoegrptb.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258.top/gtdhiqynpv.html


<!-- 参考信息 -->