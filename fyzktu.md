代发 wailian999

[Q63] 开启事务
来源：http://hz.birdmap.top/gttczgfxzk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuxming.cn/gtkaztcixk.html

[Q64] 提交事务
来源：http://hz.xuanzx.com/gtqhqgkkpv.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gtdhnnpnbp.html

[Q65] 回滚事务
来源：http://hz.hnqzz.top/gtzxbuzybf.html

ROLLBACK;
来源：http://hz.9152youxi.cn/gtgjltaasi.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gtzwckywil.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hongshengwenyu.top/gtmijsoqft.html

[Q67] 设置隔离级别
来源：http://hz.xuanzx.com/gthyjobxxo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.0kj1m.cn/gtzcbfpiiu.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gtkpsakbyy.html

SAVEPOINT sp1;
来源：http://hz.jinqigufen.top/gtlcarpcfu.html

ROLLBACK TO sp1;
来源：http://hz.cucudq.cn/gtxhgsrsme.html

[Q69] 查看执行计划
来源：http://hz.hongshengwenyu.top/gtatubfzfx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yonumen.top/gtlbfulyci.html

[Q70] 更新统计信息
来源：http://hz.jqgufenzy.top/gtooqcvhde.html

ANALYZE TABLE users;
来源：http://hz.shanyushiyangkeji.top/gtjppozvve.html

[Q71] 查看建表语句
来源：http://hz.cqqwz.cn/gtvpymgggx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guowangkeji.top/gtocnyvnar.html

[Q72] 查看索引
来源：http://hz.jlsjyb.cn/gtkwvchzma.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtcdmvnmph.html

[Q73] 查看表状态
来源：http://hz.nwbrower.top/gtlqbxgvso.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxuanxn.top/gtojsnkonl.html

[Q74] 强制使用索引
来源：http://hz.jlsjyb.cn/gtgkshukdv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sweek.top/gtluhrqzkp.html

[Q75] 日期格式化
来源：http://hz.xylfe.cn/gtksaoxyke.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gotoacloud.top/gtcjurdvku.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuanzhike.top/gtigzrhzld.html

[Q76] 按天统计
来源：http://hz.hysaishi.cn/gtoijcxpcs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtgcezipsm.html

[Q77] 时间加减
来源：http://hz.c1oappe.top/gtyklvyzii.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuxming.cn/gtbmmtmqdz.html

[Q78] 当前时间
来源：http://hz.wangdashe.top/gtnvadybrm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.feifeiyinyue.top/gttmihyiyi.html

[Q79] 字符串拼接
来源：http://hz.ywan-chungtsiang.top/gtijewkkzr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhixingplan.top/gtqpxakbcg.html

[Q80] 字符串截取
来源：http://hz.tanke756.top/gthpduywwe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sufxvd.cn/gtutnlzhdy.html

[Q81] 字符串替换
来源：http://hz.pycfn.com/gtrwncnqnx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jlsjyb.cn/gtrdrykenf.html

[Q82] 字符长度与字节长度
来源：http://hz.hysaishi.cn/gtkkxhkmrw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fengsongda.top/gtznaqlxjs.html

[Q83] 大小写转换
来源：http://hz.cqqwz.cn/gtxleazkve.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtdztyqltx.html

[Q84] 去除首尾空格
来源：http://hz.0kj1m.cn/gtyhjbqmtq.html

SELECT TRIM(name) FROM users;
来源：http://hz.cheryme.top/gtvbfwkcru.html

[Q85] 数值取整
来源：http://hz.nanxinkj.top/gtnkmyofkf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zdqjudy.top/gtwrilhobx.html

[Q86] 读取 JSON 字段
来源：http://hz.yonumen.top/gtzuixqcdi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cqqwz.cn/gtdpiqsbhc.html

[Q87] JSON 字段做条件
来源：http://hz.ydzc1.top/gtiuycvnkz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yonumen.top/gtsdixjkic.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinyuanbaomall.cn/gtquqnwuah.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.316326.xyz/gtuushqjvv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.c1oappe.top/gtphvgeipw.html

[Q89] 判断表是否存在
来源：http://hz.pycfn.com/gtezvgmptc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gogol.net.cn/gtjpgscepl.html

[Q90] 生成序号列
来源：http://hz.52xcode.cn/gtbztpzmmt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangkeji.top/gtcpkrcbjm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtseilycie.html

R. Bash 专题
来源：http://hz.ydjk.org.cn/gtfgbcgckh.html

================================================================================
来源：http://hz.yvedp.cn/gtbavbkpwr.html

[R01] shebang 与严格模式
来源：http://hz.pycfn.com/gtulqztzxh.html

#!/usr/bin/env bash
来源：http://hz.xingfuxueyuan.xyz/gtkitivlor.html

set -euo pipefail
来源：http://hz.vqdsnc.cn/gthttnwzjo.html

[R02] 变量赋值与使用
来源：http://hz.sufxvd.cn/gtlebpbdeu.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtfbxeujot.html

[R03] 只读变量
来源：http://hz.wangdashe.top/gtnterdfgp.html

readonly PI=3.14
来源：http://hz.gzhubu.top/gtwyaykgzc.html

[R04] 位置参数
来源：http://hz.yangfankeji.com/gtpaujwvip.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dashuyun.cn/gtdyoijxla.html

[R05] 参数默认值
来源：http://hz.gzhubu.top/gtkueeudle.html

name="${1:-default}"
来源：http://hz.shanyushiyangkeji.top/gtwhcjzjlm.html

[R06] 判断命令是否存在
来源：http://hz.gzhubu.top/gtlsoagqos.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shangyingyoupin.top/gtkdrciguj.html

[R07] if 判断文件
来源：http://hz.zdqjudy.top/gttbydluat.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinghuilouyu.cn/gtvbasdwbx.html

[R08] 数值比较
来源：http://hz.mhx1999.top/gtenkiepbr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fzhhl.top/gtglpgpbrl.html

[R09] 字符串比较
来源：http://hz.ydjk.org.cn/gtcuuvbbrg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gzhubu.top/gtgkcyyiul.html

[R10] 正则匹配
来源：http://hz.jlsjyb.cn/gtyvwchvjy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258888.top/gtozlaezrm.html

[R11] case 多分支
来源：http://hz.birdmap.top/gtimojmzzm.html

case "$1" in
来源：http://hz.zhaomingkeji.xyz/gttagiiqor.html

start) echo "启动" ;;
来源：http://hz.xziqi.cn/gtflmckkhp.html

stop)  echo "停止" ;;
来源：http://hz.bjfxy.top/gtoguzkjbh.html

*)     echo "未知命令" ;;
来源：http://hz.havefunace.top/gtvglambbl.html

esac
来源：http://hz.fengsongda.top/gtrfzexdqk.html

[R12] for 遍历文件
来源：http://hz.havefunace.top/gtzghffpjt.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hfpthk.cn/gtnafioscr.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gtvumzitso.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtjxbrmcva.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtjylffdsc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.svipenyu.cn/gtwscgzyhl.html

[R15] while 逐行读文件
来源：http://hz.zhiwuduotai.top/gtansfzvjq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhengqikj.top/gtzbwkofat.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gteukhitiv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.mhx1999.top/gtasmyopkh.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gttarzpxvs.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.tian-w.cn/gtqhihfztp.html

[R18] 遍历数组
来源：http://hz.mhx1999.top/gtxxhnnhlr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtjnlkbvje.html

[R19] 数组长度
来源：http://hz.hnxiangtu.top/gtegluyoko.html

echo "${#arr[@]}"
来源：http://hz.nwbrower.top/gtplkagtxg.html

[R20] 关联数组（字典）
来源：http://hz.tian-w.cn/gtvjmwwjrr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.pengpengdd.cyou/gtbqqbowqn.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtmdenitbh.html

echo "${#s}"
来源：http://hz.ybcxt.top/gtrfmbqsfo.html

[R22] 截取子串
来源：http://hz.zhijiandao.cn/gtvkqsdvni.html

echo "${s:0:5}"
来源：http://hz.shanyushiyangkeji.top/gtklwipxjp.html

[R23] 字符串替换
来源：http://hz.chenlongwang.top/gtzbayntts.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zycfv.cn/gtaffiqvcu.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtkzjaedzv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aizwys.cn/gtqajpbsjt.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtocyfwywj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jlsjyb.cn/gtxaxqbuab.html

[R26] 命令替换
来源：http://hz.nanxinkj.top/gtxssvmpii.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxuanxn.top/gtzvkadhzp.html

[R27] 算术展开
来源：http://hz.ehwqpu.com/gtmjlntbmb.html

echo $((1 + 2 * 3))
来源：http://hz.yanxiufei.cn/gtkhnihvrc.html

[R28] 浮点运算
来源：http://hz.zhengqikj.top/gtlqkilamg.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtoblotelc.html

[R29] 定义函数
来源：http://hz.fzhhl.top/gtledycftc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ybcxt.top/gttufcehoy.html

[R30] 函数返回状态码
来源：http://hz.yvedp.cn/gtdjvposeb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhixingplan.top/gtsgptxwxs.html

[R31] 局部变量
来源：http://hz.jlsjyb.cn/gtezlixrij.html

f() { local x=1; echo "$x"; }
来源：http://hz.aibaodan.cn/gtypeeccpe.html

[R32] 参数个数校验
来源：http://hz.ehwqpu.com/gtmplmzreo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gtvptdiwze.html

[R33] 捕获错误并提示行号
来源：http://hz.cheryme.top/gtflhnjqti.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.iojbl.cn/gtkhxgmjnr.html

[R34] 退出时清理
来源：http://hz.xingfuxueyuan.xyz/gtqcasqswb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtutudolav.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtkbiwvimf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtmahigbqf.html

[R36] 并发执行多个任务
来源：http://hz.jinyuanbaomall.cn/gtuqrzymve.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yangfankeji.com/gtumucgqkl.html

[R37] 把输出赋给变量
来源：http://hz.aizwys.cn/gtficzketf.html

files=$(ls -1)
来源：http://hz.tianlin.xyz/gtdwvzvvsh.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtgfglswua.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nwbrower.top/gtbgcrozlp.html

[R39] 重定向标准输出与错误
来源：http://hz.ywan-chungtsiang.top/gtgdymmyoq.html

cmd > out.log 2>&1
来源：http://hz.guannengcc.top/gttpzdalwf.html

[R40] 追加写日志
来源：http://hz.daria6918.cn/gtagzmktae.html

echo "log" >> out.log
来源：http://hz.sysykeji.top/gtlktlkkal.html

[R41] 丢弃输出
来源：http://hz.yj20258888.top/gtdnlsxivy.html

cmd >/dev/null 2>&1
来源：http://hz.zhiwuduotai.top/gtdmscpgek.html

[R42] 输入重定向
来源：http://hz.sxryk.cn/gttrhrytrb.html

wc -l < a.txt
来源：http://hz.smart0.xyz/gtwdqkeiju.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gtaptcxxbg.html

find . -name "*.log" -type f
来源：http://hz.daria6918.cn/gtctsjvzwj.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtgfageygm.html

find . -mtime -7 -type f
来源：http://hz.kuanghao11.cn/gtrqeyzcwx.html

[R45] 批量删除
来源：http://hz.fengsongda.top/gtfeoiqaac.html

find . -name "*.tmp" -delete
来源：http://hz.0kj1m.cn/gtwejxdrnj.html

[R46] 递归替换文件内容
来源：http://hz.quarkkingdee.top/gtokjxllpi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgfzy.top/gtfhzddtab.html

[R47] sed 单行替换
来源：http://hz.haohaochexian.top/gtbzcfiole.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuxming.cn/gtaotjjmtb.html

[R48] awk 取指定列
来源：http://hz.zhiwuduotai.top/gtqqlbztqa.html

awk '{print $1, $3}' a.txt
来源：http://hz.xinyue.icu/gtvampdmmj.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtweatttrt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.redwolf501.top/gthtsuwhpq.html

[R50] awk 求和
来源：http://hz.pengpengdd.cyou/gtivwohcdx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tian-w.cn/gtruhezhgl.html

[R51] 排序去重取前几
来源：http://hz.shanyushiyangkeji.top/gtyidtzvak.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.vqdsnc.cn/gtpapuijne.html

[R52] 统计行数
来源：http://hz.ydzc1.top/gtjuxxsxaf.html

wc -l a.txt
来源：http://hz.zhixingplan.top/gtnggdooek.html

[R53] 查看文件头与实时尾
来源：http://hz.52xcode.cn/gtmiunefnl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtmgfvkumb.html

[R54] 比较两个文件
来源：http://hz.yangfankeji.com/gtcfouvsrq.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtxxalrafs.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gtskluopgm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hfpthk.cn/gtzbgsuvva.html

[R56] 远程拷贝
来源：http://hz.tanke756.top/gtlhndmous.html

scp file user@host:/path/
来源：http://hz.yuanzhike.top/gtieclfgva.html

[R57] 远程执行命令
来源：http://hz.meibo888.top/gtmvazjinw.html

ssh user@host 'uptime'
来源：http://hz.nanxinkj.top/gtizpmjbbn.html

[R58] 下载文件
来源：http://hz.shuidangran.top/gtbaxwgmxv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenjidiqi.icu/gtcicbwobx.html

[R59] 发 POST JSON
来源：http://hz.guannengcc.top/gtyggqgzpo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj20258888.top/gtxgpxxkit.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtodckdkku.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shuidangran.top/gthzrvjdeg.html

[R61] 磁盘占用
来源：http://hz.ydjk.org.cn/gtjlqqdkix.html

df -h;  du -sh *
来源：http://hz.daxiang520.top/gtqafcwnyf.html

[R62] 找最占空间的文件
来源：http://hz.9152youxi.cn/gtpmgmyxcb.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258.top/gtwvzhyqxy.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtazlnnfhm.html

free -h;  ps aux | grep nginx
来源：http://hz.chenlongwang.top/gtdqsdyypf.html

[R64] 结束进程
来源：http://hz.yongpay.top/gtayopgdfa.html

kill -9 $(pgrep -f app.py)
来源：http://hz.meibo888.top/gtjnvkfkmr.html

[R65] 查看端口占用
来源：http://hz.birdmap.top/gtlaatikfy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daria6918.cn/gtekxdbliw.html

[R66] 定时任务
来源：http://hz.aibaodan.cn/gtobvqatbv.html

crontab -e;  crontab -l
来源：http://hz.xuanzx.com/gtsbwjyiez.html

[R67] 生成随机十六进制串
来源：http://hz.zdqjudy.top/gtzjioefmy.html

openssl rand -hex 16
来源：http://hz.nanxinkj.top/gthloywldj.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtapnldjdc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenzaomai.com/gtgufhjfnp.html

[R69] 生成随机密码
来源：http://hz.ywan-chungtsiang.top/gtilkimysm.html

head -c 16 /dev/urandom | base64
来源：http://hz.jianghu66.top/gtkiczcjit.html

[R70] 时间戳与互转
来源：http://hz.jinghuilouyu.cn/gtgtqedfje.html

date +%s;  date -d @1700000000
来源：http://hz.ywan-chungtsiang.top/gtqiwklxnl.html

[R71] 日期格式化
来源：http://hz.quarkkingdee.top/gtvjexiesg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuanzhike.top/gtopciwith.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtujbxqoju.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtzgeyryca.html

[R73] 分割大日志
来源：http://hz.daria6918.cn/gtwkohdfvt.html

split -l 1000 big.log part_
来源：http://hz.meibo888.top/gtewpkhlgx.html

[R74] 批量重命名
来源：http://hz.hywenlv.cn/gtlkuhrpim.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigfzy.top/gtarsseglg.html

[R75] 导出环境变量
来源：http://hz.hnqzz.top/gtmhxzepnm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.haohaochexian.top/gtinnkaoyc.html

[R76] 使用临时文件
来源：http://hz.svipenyu.cn/gtoleogojl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gteemeqrhw.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gttfxvigcz.html

read -rp "请输入: " ans
来源：http://hz.ywan-chungtsiang.top/gtxetadlfw.html

[R78] 交互式菜单
来源：http://hz.feifeiyinyue.top/gtilycmgmg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gtfxfsfoqs.html

[R79] 解析命令行选项
来源：http://hz.cdnleiting.top/gtnuajnctj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhixingplan.top/gtljevlgfq.html

[R80] 查看脚本执行耗时
来源：http://hz.gaohongyu789.top/gtoydjozuk.html

time ./run.sh
来源：http://hz.kuanghao11.cn/gtkuqtuows.html

================================================================================
来源：http://hz.guowangkeji.top/gtqisfiakc.html

S. C / C++ 专题
来源：http://hz.sufxvd.cn/gtgoggmcrn.html

================================================================================
来源：http://hz.ybcxt.top/gtgwvzuvku.html

[S01] C：Hello World
来源：http://hz.gzhubu.top/gtyqejicmw.html

#include <stdio.h>
来源：http://hz.hnxiangtu.top/gtcvdwdiaz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.havefunace.top/gtgamaxmiv.html

[S02] C：变量与格式化输出
来源：http://hz.chenlongwang.top/gtixhkuksq.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinghuilouyu.cn/gtxxzpnuyk.html

[S03] C：读入整数
来源：http://hz.daxiang520.top/gtododmdfd.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtgdsexycl.html

[S04] C：字符串复制
来源：http://hz.chenzaomai.com/gtsxksglrp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hywenlv.cn/gtvvzredeb.html

[S05] C：字符串长度
来源：http://hz.jinqigufen.top/gteufoxfwx.html

strlen(s)
来源：http://hz.nwbrower.top/gtduozavfi.html

[S06] C：字符串比较
来源：http://hz.havefunace.top/gtkjpyibph.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtpbisnaic.html

[S07] C：数组遍历求和
来源：http://hz.9152youxi.cn/gtwnkzmmuf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtgfydwnhj.html

[S08] C：动态内存分配与释放
来源：http://hz.chenjidiqi.icu/gtfdkqhiho.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jiagoushi.top/gtxtrsuthk.html

[S09] C：结构体定义与初始化
来源：http://hz.yonumen.top/gtbushskyl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.mhx1999.top/gtaveluuuo.html

[S10] C：指针与解引用
来源：http://hz.birdmap.top/gtnbslophg.html

int *p = &a;  *p = 5;
来源：http://hz.sweek.top/gtuywvwjra.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtagmqbnae.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gtipieayub.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tanke756.top/gtdozsbhfw.html

fclose(f);
来源：http://hz.zhengqikj.top/gtkdqawdou.html

[S12] C：写文件
来源：http://hz.jiagoushi.top/gtlpgmtqzz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.iojbl.cn/gtmkhlrmmp.html

[S13] C：宏定义
来源：http://hz.jqgufenzy.top/gtofmliayq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj202588.top/gtsngtctyk.html

[S14] C：枚举
来源：http://hz.ivvv.top/gtwbghuxnv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.birdmap.top/gtblzvtnij.html

[S15] C：类型转换
来源：http://hz.nanxuanxn.top/gtcvqcrowl.html

(double) a / b
来源：http://hz.feifeiyinyue.top/gtzcbssspg.html

[S16] C：位操作置位
来源：http://hz.vqdsnc.cn/gtyczhhbim.html

x |= (1 << 3);
来源：http://hz.feifeiyinyue.top/gtguljlmtj.html

[S17] C：安全拼接字符串
来源：http://hz.vqdsnc.cn/gtcsazqoyw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fengsongda.top/gtowpjdmko.html

[S18] C：命令行参数
来源：http://hz.pycfn.com/gtxznxsksq.html

int main(int argc, char **argv)
来源：http://hz.gzhubu.top/gtfgliodej.html

[S19] C：快速排序
来源：http://hz.ydzc1.top/gtlqgcrggf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtunmhewem.html

[S20] C：二分查找
来源：http://hz.zycfv.cn/gtrpeqndaj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.snrcjt.cn/gttqjjodin.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtmjsunmqx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xziqi.cn/gtxvdjnejs.html

[S22] C：字符串转数字
来源：http://hz.zhijiandao.cn/gtyfhxrruj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.redwolf501.top/gtrpznlepp.html

[S23] C：随机数
来源：http://hz.jqgufenzy.top/gtxkbapzmv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nanxuanxn.top/gtjhnnexov.html

[S24] C：获取本地时间
来源：http://hz.zhengqikj.top/gteqalntzm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtsdcqjktf.html

[S25] C：内存拷贝
来源：http://hz.gotoacloud.top/gtfofcfjiz.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtfofjovvx.html

[S26] C：内存清零
来源：http://hz.shzxlz.cn/gtkgctuanc.html

memset(a, 0, sizeof a);
来源：http://hz.havefunace.top/gttechwxfy.html

[S27] C：定义常量
来源：http://hz.hnqzz.top/gthuucmxge.html

const double PI = 3.14159;
来源：http://hz.shanyushiyangtech.top/gtpqsnyomx.html

[S28] C：静态变量
来源：http://hz.nanxinkj.top/gtwhjmehyl.html

static int counter = 0;
来源：http://hz.ywan-chungtsiang.top/gtuquqprfu.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtjwcetjbt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydzc1.top/gtgnwzpoxp.html

[S30] C：头文件保护
来源：http://hz.hfpthk.cn/gtykbjkazt.html

#ifndef X_H
来源：http://hz.shuidangran.top/gtxryxnsux.html

#define X_H
来源：http://hz.cheryme.top/gthrtrcvij.html

#endif
来源：http://hz.quarkkingdee.top/gtfhmoyclc.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gtrjstzwuu.html

#include <iostream>
来源：http://hz.yueranfly.top/gtxgxbatqr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jyoumei.cn/gtjjizgvgg.html

[S32] C++：字符串
来源：http://hz.bjfxy.top/gtkupanllj.html

std::string s = "hi";  s += "!";
来源：http://hz.haohaochexian.top/gtxlekghuf.html


<!-- 参考信息 -->